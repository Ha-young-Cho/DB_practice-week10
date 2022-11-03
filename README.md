# INHA-DB
DB설계 week10 실습

1. 레포지토리 복사

i. git clone <원격저장소 주소>
ii. 해당 폴더 이동 (ex) cd week10
iii. npm install
iv. npm run start

2. database/sql.js 파일 내부에서 본인의 데이터베이스 정보 입력

const pool = mysql.createPool(
    process.env.JAWSDB_URL ?? {
        host: 'localhost',
        user: 'root',
        database : "week10",
        password: 'hyoungm41004!',
        waitForConnections: true,
        connectionLimit: 10,
        queueLimit:0,
    }
);
