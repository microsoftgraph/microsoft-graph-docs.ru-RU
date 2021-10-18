---
title: Запись данных в книгу Excel с помощью Microsoft Graph
description: q=excelstarter).
ms.localizationpriority: high
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 266427ed2853c26a2267b043b84e04f346467ab2
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457115"
---
# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a>Запись данных в книгу Excel с помощью Microsoft Graph

REST API для Excel обеспечивает простой независимый от платформ способ отправки информации в книгу Excel. В этой статье рассказывается, как записать простые наборы данных в книгу Excel в трех платформах веб-разработки: ASP.NET, Angular и React. Примеры кода, о которых рассказывается в этой статье, см. на веб-странице [примеров по работе с Excel и Microsoft Graph для начинающих на веб-сайте GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter).

> **Примечание.** Во всех трех примерах показано, как записывать данные в книгу Excel с именем **demo.xlsx**. Вы можете отправить книгу из этих примеров в свой OneDrive. Кроме того, для отправки файлов в OneDrive можно использовать Microsoft Graph. Если вы хотите изучить вызовы REST, вам потребуется отправить файл любого типа в корневую папку вашего OneDrive. См. [пример списка задач ASP.NET для REST API Microsoft Graph](https://github.com/microsoftgraph/aspnet-todo-rest-sample).

Все три примера работы с Excel для начинающих делают одно и то же: получают имя и адрес пользователя, вошедшего в систему, и добавляют эти сведения в новую строку в книге **demo.xlsx**. Вы можете изменить примеры так, чтобы код добавлял дополнительные строки путем простого добавления информации в двумерный массив, представляющий строку или строки, которые вы хотите добавить.

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a>Добавление одной или нескольких строк в книгу Excel с помощью одного запроса REST

При использовании REST API для Excel от вас требуется отправить простой запрос POST в конечную точку REST, которая представляет коллекцию строк книги Excel. Если вы работаете с записной книжкой в корневой папке учетной записи OneDrive пользователя, вошедшего в систему, конечная точка REST будет выглядеть указанным ниже образом.

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

Дополнительные сведения о том, как получить доступ к файлам в папках OneDrive, см. в разделе [Тип ресурса DriveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) в нашей справочной документации.

> **Примечание.** Вы можете просмотреть существующую коллекцию строк книги, отправив запрос GET по части пути, который заканчивается на `/rows`.

Текст запроса POST выглядит указанным ниже образом.

```json
{
  "index": null,
  "values": [
    ["alex darrow", "adarrow@tenant.onmicrosoft.com"]
  ]
}
```

Значение первого параметра `index` указывает относительное положение строки, которую вы добавляете в массив строк, нумерация элементов которого начинается с нуля. Строки, расположенные ниже вставляемой строки, будут сдвинуты вниз. Параметр `null` указывает, что новая строка будет добавлена в конец.

Значение второго параметра `values` представляет собой двумерный строковый массив, содержащий неформатированные значения всех строк, которые вы хотите добавить. Массив, приведенный в примере, содержит только одну строку, но вы можете добавить дополнительные строки. Для этого добавьте дополнительные строковые массивы.

Вы можете протестировать этот запрос в своей учетной записи OneDrive, отправив файл demo.xlsx в корневую папку OneDrive и выполнив этот запрос в [песочнице Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).

Это все, что вам нужно знать, чтобы записывать данные в книгу Excel. Вам необходимо знать, как создавать запрос в используемой вами платформе, и в примерах по работе с Excel для начинающих продемонстрированы три способа решения этой задачи.

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a>Добавление одной или нескольких строк в книгу Excel в ASP.NET

Код ASP.NET для создания и отправки запросов см. в файлах [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) и [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) в [примере по работе с Excel в Microsoft Graph для ASP.NET 4.6 для начинающих](https://github.com/microsoftgraph/aspnet-excelstarter-sample).

В файле `GraphResources.cs` есть вспомогательный класс для инкапсуляции пользовательских данных, которые вы получаете из Microsoft Graph, и тело запроса, которое вы будете использовать для записи данных в книгу.

```csharp
public class UserInfo
{
    public string Name { get; set; }
    public string Address { get; set; }

}

public class UserInfoRequest
{
    public string index { get; set; }
    public string[][] values { get; set; }
}
```

Класс `GraphService.cs` содержит метод `AddInfoToExcel`, который заполняет эти классы, сериализует информацию в запросе в объект JSON, а затем передает этот объект в качестве тела запроса POST.

```csharp
public async Task<string> AddInfoToExcel(string accessToken, string name, string address)
{
    string endpoint = "https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add";
    using (var client = new HttpClient())
    {
        using (var request = new HttpRequestMessage(HttpMethod.Post, endpoint))
        {
            // Populate UserInfoRequest object
            string[] userInfo = { name, address  };
            string[][] userInfoArray = { userInfo };
            UserInfoRequest userInfoRequest = new UserInfoRequest();
            userInfoRequest.index = null;
            userInfoRequest.values = userInfoArray;

            // Serialize the information in the UserInfoRequest object
            string jsonBody = JsonConvert.SerializeObject(userInfoRequest);
            request.Headers.Accept.Add(new MediaTypeWithQualityHeaderValue("application/json"));
            request.Headers.Authorization = new AuthenticationHeaderValue("Bearer", accessToken);
            request.Content = new StringContent(jsonBody, Encoding.UTF8, "application/json");

            using (var response = await client.SendAsync(request))
            {
                if (response.IsSuccessStatusCode)
                {
                    return Resource.Graph_UploadToExcel_Success_Result;
                }
                return response.ReasonPhrase;
            }
        }
    }
}
```

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a>Добавление одной или нескольких строк в книгу Excel в Angular

Код Angular для создания и отправки запросов см. в файле [home.service.ts](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) в [примере по работе с Excel в Microsoft Graph для Angular для начинающих](https://github.com/microsoftgraph/angular-excelstarter-sample).

Так как в этом примере применяется TypeScript, в нем используется [клиентская библиотека JavaScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) и [типы TypeScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-typescript-typings).

Функция `addInfoToExcel` в файле `home.service.ts` создает двумерный строковый массив и тело запроса, содержащее массив. Затем с помощью клиентской библиотеки JavaScript для Microsoft Graph она создает и отправляет запрос. Ответ возвращается в виде обещания.

```typescript
addInfoToExcel(user: MicrosoftGraph.User) {
  const userInfo = [];
  const userEmail = user.mail || user.userPrincipalName;
  userInfo.push([user.displayName, userEmail]);

  const userInfoRequestBody = {
    index: null,
    values: userInfo
  };

  const body = JSON.stringify(userInfoRequestBody);

  var client = this.getClient();
  var url = `${this.url}/me/drive/root:/${this.file}:/workbook/tables/${this.table}/rows/add`
  return Observable.fromPromise(client
  .api(url)
  .post(body)
  );
}
```

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a>Добавление одной или нескольких строк в книгу Excel в React

Код для создания и отправки запросов см. в файле [home.js](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) в [примере по работе с Excel в Microsoft Graph для React для начинающих](https://github.com/microsoftgraph/react-excelstarter-sample).

Функция `onWriteToExcel` создает двумерный строковый массив и передает его в виде тела запроса. Для осуществления HTTP-запроса в ней используется [axios](https://www.npmjs.com/package/axios).

```typescript
onWriteToExcel() {
  const { token, me } = this.state;

  const myEmailAddress = me.mail || me.userPrincipalName;
  const values = [];

  values.push([me.displayName, myEmailAddress]);

  axios
    .post('https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add',
      { index: null, values },
      { headers: { Authorization: `Bearer ${token}` }}
    )
    .then(res => {
                    console.log(res);
                    const successMessage = "Successfully wrote your data to demo.xlsx!";
                    this.setState ({ successMessage });
                    })
    .catch(err => console.error(err));
}
```

## <a name="see-also"></a>См. также

* [Управление сеансами в Excel с помощью Microsoft Graph](excel-manage-sessions.md)
* [Использование функций книг в Excel с помощью Microsoft Graph](excel-use-functions.md)
* [Обновление формата диапазона в Excel с помощью Microsoft Graph](excel-update-range-format.md)
* [Показ изображения диаграммы в Excel с помощью Microsoft Graph](excel-display-chart-image.md)
* [Использование REST API для Excel](/graph/api/resources/excel?view=graph-rest-1.0)
