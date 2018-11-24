# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="6a163-101">Список опубликованных приложений из каталога приложений группами Майкрософт</span><span class="sxs-lookup"><span data-stu-id="6a163-101">List the published apps from the Microsoft Teams app catalog</span></span>



<span data-ttu-id="6a163-102">Список [приложений](../resources/teamsapp.md) из каталога приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="6a163-102">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="6a163-103">Этот компонент включает приложений из магазина группами Майкрософт, а также приложений из каталога приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="6a163-103">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="6a163-104">Приобретать приложения в вашей организации только каталог приложений, укажите `Organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6a163-104">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a163-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a163-105">Permissions</span></span>

<span data-ttu-id="6a163-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="6a163-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="6a163-108">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="6a163-108">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="6a163-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a163-109">Permission Type</span></span>                        | <span data-ttu-id="6a163-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a163-110">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="6a163-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a163-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a163-112">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a163-112">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="6a163-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a163-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a163-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a163-114">Not supported</span></span>|
| <span data-ttu-id="6a163-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a163-115">Application</span></span>                            | <span data-ttu-id="6a163-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6a163-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a163-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a163-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a163-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a163-118">Optional query parameters</span></span>
<span data-ttu-id="6a163-119">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6a163-119">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a163-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a163-120">Request headers</span></span>

| <span data-ttu-id="6a163-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a163-121">Header</span></span>        | <span data-ttu-id="6a163-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6a163-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="6a163-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a163-123">Authorization</span></span> | <span data-ttu-id="6a163-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a163-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6a163-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a163-126">Request body</span></span>
<span data-ttu-id="6a163-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6a163-127">None.</span></span>

><span data-ttu-id="6a163-128">**Примечание:** Можно отфильтровать поля объекта [teamsCatalogApp](../resources/teamsapp.md) для сокращения списка результатов.</span><span class="sxs-lookup"><span data-stu-id="6a163-128">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="6a163-129">Можно использовать любой из следующих операций фильтра: равно, не равно и, или, а не.</span><span class="sxs-lookup"><span data-stu-id="6a163-129">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="6a163-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a163-130">Response</span></span>
<span data-ttu-id="6a163-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [teamsCatalogApp](../resources/teamsapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6a163-131">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a163-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="6a163-132">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="6a163-133">Пример 1</span><span class="sxs-lookup"><span data-stu-id="6a163-133">Example 1</span></span>
<span data-ttu-id="6a163-134">В следующем примере перечисляются все приложения, которые специфичны для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="6a163-134">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="6a163-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a163-135">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="6a163-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a163-136">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="6a163-137">Пример 2</span><span class="sxs-lookup"><span data-stu-id="6a163-137">Example 2</span></span>

<span data-ttu-id="6a163-138">В следующем примере перечисляются приложений с указанным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="6a163-138">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="6a163-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a163-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="6a163-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a163-140">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

