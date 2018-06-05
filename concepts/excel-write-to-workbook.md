# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a><span data-ttu-id="70bd2-101">Запись данных в книгу Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="70bd2-101">Write data to an Excel workbook with Microsoft Graph</span></span>

<span data-ttu-id="70bd2-102">REST API для Excel обеспечивает простой независимый от платформ способ отправки информации в книгу Excel.</span><span class="sxs-lookup"><span data-stu-id="70bd2-102">The Excel REST API provides an easy, platform-agnostic way to upload information to an Excel workbook.</span></span> <span data-ttu-id="70bd2-103">В этой статье рассказывается, как записать простые наборы данных в книгу Excel в трех платформах веб-разработки: ASP.NET, Angular и React.</span><span class="sxs-lookup"><span data-stu-id="70bd2-103">This topic shows you how to write simple data sets to an Excel workbook on three web development frameworks: ASP.NET, Angular, and React.</span></span> <span data-ttu-id="70bd2-104">Примеры кода, о которых рассказывается в этой статье, см. на веб-странице [примеров по работе с Excel и Microsoft Graph для начинающих на веб-сайте GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter).</span><span class="sxs-lookup"><span data-stu-id="70bd2-104">You can look at the code samples featured in this topic by visiting the [Microsoft Graph Excel starter samples on GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter).</span></span>

> <span data-ttu-id="70bd2-105">**Примечание.** Во всех трех примерах показано, как записывать данные в книгу Excel с именем **demo.xlxs**.</span><span class="sxs-lookup"><span data-stu-id="70bd2-105">**Note:** All three of the samples write data to an Excel workbook named **demo.xlxs**.</span></span> <span data-ttu-id="70bd2-106">Вы можете отправить книгу из этих примеров в свой OneDrive. Кроме того, для отправки файлов в OneDrive можно использовать Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70bd2-106">They provide this workbook for you so that you can upload it to your own OneDrive, but you can also use Microsoft Graph to upload files to OneDrive.</span></span> <span data-ttu-id="70bd2-107">Если вы хотите изучить вызовы REST, вам потребуется отправить файл любого типа в корневую папку вашего OneDrive. См. [пример списка задач ASP.NET для REST API Microsoft Graph](https://github.com/microsoftgraph/aspnet-todo-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="70bd2-107">If you're interested in learning the REST calls you need to upload a file of any type to your root OneDrive folder, see the [Microsoft Graph Excel REST API ASP.NET to-do list sample](https://github.com/microsoftgraph/aspnet-todo-rest-sample).</span></span>

<span data-ttu-id="70bd2-108">Все три примера работы с Excel для начинающих делают одно и то же: получают имя и адрес пользователя, вошедшего в систему, и добавляют эти сведения в новую строку в книге **demo.xlsx**.</span><span class="sxs-lookup"><span data-stu-id="70bd2-108">All three of the Excel starter samples do the same thing: retrieve the name and address of the signed-in user and add those two pieces of information to a new row in the **demo.xlsx** workbook.</span></span> <span data-ttu-id="70bd2-109">Вы можете изменить примеры так, чтобы код добавлял дополнительные строки путем простого добавления информации в двумерный массив, представляющий строку или строки, которые вы хотите добавить.</span><span class="sxs-lookup"><span data-stu-id="70bd2-109">You can modify the samples to add additional rows simply by adding information to the two-dimensional array that represents the row or rows that you want to add.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a><span data-ttu-id="70bd2-110">Добавление одной или нескольких строк в книгу Excel с помощью одного запроса REST</span><span class="sxs-lookup"><span data-stu-id="70bd2-110">Add a row or rows to an Excel workbook with a single REST request</span></span>

<span data-ttu-id="70bd2-111">При использовании REST API для Excel от вас требуется отправить простой запрос POST в конечную точку REST, которая представляет коллекцию строк книги Excel.</span><span class="sxs-lookup"><span data-stu-id="70bd2-111">The Excel REST API requires you to POST a simple request body to the REST endpoint that represents the row collection of an Excel workbook.</span></span> <span data-ttu-id="70bd2-112">Если вы работаете с записной книжкой в корневой папке учетной записи OneDrive пользователя, вошедшего в систему, конечная точка REST будет выглядеть указанным ниже образом.</span><span class="sxs-lookup"><span data-stu-id="70bd2-112">If you're working with a notebook in the root folder of the signed-in user's OneDrive account, the REST endpoint will look like this:</span></span>

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

<span data-ttu-id="70bd2-113">Дополнительные сведения о том, как получить доступ к файлам в папках OneDrive, см. в разделе [Тип ресурса DriveItem](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/driveitem) в нашей справочной документации.</span><span class="sxs-lookup"><span data-stu-id="70bd2-113">For more information about how to reach files in OneDrive folders, see the [DriveItem resource type](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/driveitem) in our reference documentation.</span></span>

> <span data-ttu-id="70bd2-114">**Примечание.** Вы можете просмотреть существующую коллекцию строк книги, отправив запрос GET по части пути, который заканчивается на `/rows`.</span><span class="sxs-lookup"><span data-stu-id="70bd2-114">**Note:** You can look at the existing row collection of the workbook by making a GET request to the part of the path that ends at `/rows`.</span></span>

<span data-ttu-id="70bd2-115">Текст запроса POST выглядит указанным ниже образом.</span><span class="sxs-lookup"><span data-stu-id="70bd2-115">The POST body looks like this:</span></span>

`{
  "index": null,
  "values": [
    ['alex darrow', 'adarrow@tenant.onmicrosoft.com']
  ]
}`

<span data-ttu-id="70bd2-116">Значение первого параметра `index` указывает относительное положение строки, которую вы добавляете в массив строк, нумерация элементов которого начинается с нуля.</span><span class="sxs-lookup"><span data-stu-id="70bd2-116">The value of the first `index` parameter specifies the relative position of the row that you're adding to the zero-indexed array of rows.</span></span> <span data-ttu-id="70bd2-117">Строки, расположенные ниже вставляемой строки, будут сдвинуты вниз.</span><span class="sxs-lookup"><span data-stu-id="70bd2-117">Rows below the inserted row will be shifted downwards.</span></span> <span data-ttu-id="70bd2-118">Параметр `null` указывает, что новая строка будет добавлена в конец.</span><span class="sxs-lookup"><span data-stu-id="70bd2-118">The `null` parameter indicates that the new row will be added to the end.</span></span>

<span data-ttu-id="70bd2-119">Значение второго параметра `values` представляет собой двумерный строковый массив, содержащий неформатированные значения всех строк, которые вы хотите добавить.</span><span class="sxs-lookup"><span data-stu-id="70bd2-119">The value of the second `values` parameter is a two-dimensional string array that contains the unformatted values of each row that you want to add.</span></span> <span data-ttu-id="70bd2-120">Массив, приведенный в примере, содержит только одну строку, но вы можете добавить дополнительные строки. Для этого добавьте дополнительные строковые массивы.</span><span class="sxs-lookup"><span data-stu-id="70bd2-120">The array in the sample contains only one row, but you can add more rows by adding more string arrays.</span></span>

<span data-ttu-id="70bd2-121">Вы можете протестировать этот запрос в своей учетной записи OneDrive, отправив файл demo.xlsx в корневую папку OneDrive и выполнив этот запрос в [песочнице Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="70bd2-121">You can test this query with your own OneDrive account by uploading the demo.xlsx file to your OneDrive root folder and executing this query on the [Microsoft Graph Explorer](https://developer.microsoft.com/ru-RU/graph/graph-explorer).</span></span>

<span data-ttu-id="70bd2-122">Это все, что вам нужно знать, чтобы записывать данные в книгу Excel.</span><span class="sxs-lookup"><span data-stu-id="70bd2-122">That is all you need to know in order to write data to an Excel workbook.</span></span> <span data-ttu-id="70bd2-123">Вам необходимо знать, как создавать запрос в используемой вами платформе, и в примерах по работе с Excel для начинающих продемонстрированы три способа решения этой задачи.</span><span class="sxs-lookup"><span data-stu-id="70bd2-123">You do need to know how to construct and make the request in your own framework, and the Excel starter samples demonstrate three separate ways of doing this.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a><span data-ttu-id="70bd2-124">Добавление одной или нескольких строк в книгу Excel в ASP.NET</span><span class="sxs-lookup"><span data-stu-id="70bd2-124">Add a row or rows to an Excel workbook in ASP.NET</span></span>

<span data-ttu-id="70bd2-125">Код ASP.NET для создания и отправки запросов см. в файлах [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) и [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) в [примере по работе с Excel в Microsoft Graph для ASP.NET 4.6 для начинающих](https://github.com/microsoftgraph/aspnet-excelstarter-sample).</span><span class="sxs-lookup"><span data-stu-id="70bd2-125">You'll find the ASP.NET code that constructs and sends the request in the [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) and [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) files of the [Microsoft Graph Excel Starter Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-excelstarter-sample).</span></span>

<span data-ttu-id="70bd2-126">В файле `GraphResources.cs` есть вспомогательный класс для инкапсуляции пользовательских данных, которые вы получаете из Microsoft Graph, и тело запроса, которое вы будете использовать для записи данных в книгу.</span><span class="sxs-lookup"><span data-stu-id="70bd2-126">The `GraphResources.cs` file provides a helper class for encapsulating both the user data you're retrieving from Microsoft Graph and the request body that you'll use when you write to your workbook.</span></span>

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

<span data-ttu-id="70bd2-127">Класс `GraphService.cs` содержит метод `AddInfoToExcel`, который заполняет эти классы, сериализует информацию в запросе в объект JSON, а затем передает этот объект в качестве тела запроса POST.</span><span class="sxs-lookup"><span data-stu-id="70bd2-127">The `GraphService.cs` class contains an `AddInfoToExcel` method that populates these classes, serializes the request information into a JSON object, and then passes that object as the POST request body.</span></span>

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

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a><span data-ttu-id="70bd2-128">Добавление одной или нескольких строк в книгу Excel в Angular</span><span class="sxs-lookup"><span data-stu-id="70bd2-128">Add a row or rows to an Excel workbook in Angular</span></span>

<span data-ttu-id="70bd2-129">Код Angular для создания и отправки запросов см. в файле [home.service.ts](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) в [примере по работе с Excel в Microsoft Graph для Angular для начинающих](https://github.com/microsoftgraph/angular-excelstarter-sample).</span><span class="sxs-lookup"><span data-stu-id="70bd2-129">You'll find the Angular code that constructs and sends the request in the [home.service.ts file](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) of the [Microsoft Graph Excel Starter Sample for Angular](https://github.com/microsoftgraph/angular-excelstarter-sample).</span></span>

<span data-ttu-id="70bd2-130">Так как в этом примере применяется TypeScript, в нем используется [клиентская библиотека JavaScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) и [типы TypeScript для Microsoft Graph](https://github.com/microsoftgraph/msgraph-typescript-typings).</span><span class="sxs-lookup"><span data-stu-id="70bd2-130">Since this sample uses TypeScript, it takes advantage of the [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) and the [ Microsoft Graph TypeScript Types](https://github.com/microsoftgraph/msgraph-typescript-typings).</span></span>

<span data-ttu-id="70bd2-131">Функция `addInfoToExcel` в файле `home.service.ts` создает двумерный строковый массив и тело запроса, содержащее массив.</span><span class="sxs-lookup"><span data-stu-id="70bd2-131">The `addInfoToExcel` function in the `home.service.ts` file constructs the two-dimensional string array and the request body that contains the array.</span></span> <span data-ttu-id="70bd2-132">Затем с помощью клиентской библиотеки JavaScript для Microsoft Graph она создает и отправляет запрос.</span><span class="sxs-lookup"><span data-stu-id="70bd2-132">It then uses the Microsoft Graph JavaScript Client Library to construct and send the request.</span></span> <span data-ttu-id="70bd2-133">Ответ возвращается в виде обещания.</span><span class="sxs-lookup"><span data-stu-id="70bd2-133">The response comes back in the form of a Promise.</span></span>

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

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a><span data-ttu-id="70bd2-134">Добавление одной или нескольких строк в книгу Excel в React</span><span class="sxs-lookup"><span data-stu-id="70bd2-134">Add a row or rows to an Excel workbook in React</span></span>

<span data-ttu-id="70bd2-135">Код для создания и отправки запросов см. в файле [home.js](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) в [примере по работе с Excel в Microsoft Graph для React для начинающих](https://github.com/microsoftgraph/react-excelstarter-sample).</span><span class="sxs-lookup"><span data-stu-id="70bd2-135">You'll find the code that constructs and sends the request in the [home.js file](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) of the [Microsoft Graph Excel Starter Sample for React](https://github.com/microsoftgraph/react-excelstarter-sample).</span></span>

<span data-ttu-id="70bd2-136">Функция `onWriteToExcel` создает двумерный строковый массив и передает его в виде тела запроса.</span><span class="sxs-lookup"><span data-stu-id="70bd2-136">The `onWriteToExcel` function constructs the two-dimensional string array and passes it as the request body.</span></span> <span data-ttu-id="70bd2-137">Для осуществления HTTP-запроса в ней используется [axios](https://www.npmjs.com/package/axios).</span><span class="sxs-lookup"><span data-stu-id="70bd2-137">It uses [axios](https://www.npmjs.com/package/axios) to make the HTTP request.</span></span>

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

##<a name="see-also"></a><span data-ttu-id="70bd2-138">См. также</span><span class="sxs-lookup"><span data-stu-id="70bd2-138">See also</span></span>

* [<span data-ttu-id="70bd2-139">Управление сеансами в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="70bd2-139">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="70bd2-140">Использование функций книг в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="70bd2-140">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="70bd2-141">Обновление формата диапазона в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="70bd2-141">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="70bd2-142">Показ изображения диаграммы в Excel с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="70bd2-142">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="70bd2-143">Использование REST API для Excel</span><span class="sxs-lookup"><span data-stu-id="70bd2-143">Use the Excel REST API</span></span>](../api-reference/v1.0/resources/excel.md)    
