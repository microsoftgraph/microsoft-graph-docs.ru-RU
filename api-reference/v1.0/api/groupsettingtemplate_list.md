# <a name="list-groupsettingtemplates"></a><span data-ttu-id="48bba-101">Перечисление объектов groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="48bba-101">List groupSettingTemplates</span></span>

<span data-ttu-id="48bba-p101">Шаблоны параметров группы представляют набор шаблонов, на базе которых можно создавать параметры группы для использования в клиенте.  Эта операция позволяет получить список доступных объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="48bba-p101">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="48bba-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48bba-104">Permissions</span></span>

<span data-ttu-id="48bba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48bba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="48bba-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48bba-107">Permission type</span></span>      | <span data-ttu-id="48bba-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48bba-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48bba-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48bba-109">Delegated (work or school account)</span></span> | <span data-ttu-id="48bba-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48bba-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48bba-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48bba-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48bba-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48bba-112">Not supported.</span></span>    |
|<span data-ttu-id="48bba-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48bba-113">Application</span></span> | <span data-ttu-id="48bba-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48bba-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48bba-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48bba-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="48bba-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48bba-116">Optional query parameters</span></span>
<span data-ttu-id="48bba-117">Этот метод поддерживает [параметры запросов OData](http://graph.microsoft.io/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="48bba-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="48bba-118">**Примечание.** $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48bba-118">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48bba-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48bba-119">Request headers</span></span>
| <span data-ttu-id="48bba-120">Имя</span><span class="sxs-lookup"><span data-stu-id="48bba-120">Name</span></span> | <span data-ttu-id="48bba-121">Описание</span><span class="sxs-lookup"><span data-stu-id="48bba-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="48bba-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48bba-122">Authorization</span></span>  | <span data-ttu-id="48bba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48bba-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48bba-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48bba-125">Request body</span></span>
<span data-ttu-id="48bba-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48bba-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48bba-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="48bba-127">Response</span></span>

<span data-ttu-id="48bba-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupSettingTemplate](../resources/groupsettingtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="48bba-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48bba-129">Пример</span><span class="sxs-lookup"><span data-stu-id="48bba-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48bba-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="48bba-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="48bba-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="48bba-131">Response</span></span>

<span data-ttu-id="48bba-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48bba-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
                    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
                    "deletedDateTime": null,
                    "displayName": "Group.Unified",
                    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
                    "values": [
                        {
                            "name": "CustomBlockedWordsList",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "EnableMSStandardBlockedWords",
                            "type": "System.Boolean",
                            "defaultValue": "false",
                            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
                        },
                        {
                            "name": "ClassificationDescriptions",
                            "type": "System.String",
                            "defaultValue": "",
                            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
                        }
                }
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->