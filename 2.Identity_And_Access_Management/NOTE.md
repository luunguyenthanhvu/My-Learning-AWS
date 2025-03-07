# Giới thiệu về IAM và kiểm soát hành vi người dùng và các chính sách truy cập IAM

<details>
 <summary>
  <b>Phân Quyền (Permissions): </b>
 </summary>
  
  - Chúng ta cấp các quyền hạn sử dụng policy documents, policy documents được tạo từ ngôn ngữ JSON (JavaScript Object Notation).
    - Ví dụ của một Policy Document (một ví dụ của một admin)
    ```json
    {
        "Version": "2012-10-17",
            "Statement":{
                "Efect":"Allow",
                "Action":"*",
                "Resource":"*",
            }
    }
    ```
    - <b> IAM POLICY DOCUMENTS: </b> Cấp quyền cho:
      - Group (Nên cấp cho group).
      - User (Trên thực tế không nên cấp cho user mà user sẽ sử dụng policy documents thông qua group để thực hiện quyền truy cập vào AWS cloud).
      - Role (có thể thừa kế IAM Policy documents -> gắn quyền cho User hay group, hoặc một dịch vụ như EC2, Lamda.....).
  - 
</details>