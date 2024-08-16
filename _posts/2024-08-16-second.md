class Professor:
    def __init__(self, name, department, university, interests):
        self.name = name
        self.department = department
        self.university = university
        self.interests = interests

    def introduce(self):
        print(f"안녕하세요, 저는 {self.university}의 {self.department} 교수 {self.name}입니다.")
        print("저의 주요 관심사는 다음과 같습니다:")
        for interest in self.interests:
            print(f"- {interest}")

if __name__ == "__main__":
    name = "김태완"  # 여기에 본인의 이름을 입력하세요.
    department = "중어중문학과"
    university = "국립 전남대학교"
    interests = [
        "한자의 구조 연구",
        "데이터 분석",
        "미술 이론",
        "전시 및 기획"
    ]

    professor = Professor(name, department, university, interests)
    professor.introduce()
