# <a name="create-sectiongroup"></a><span data-ttu-id="308e9-101">Создание sectionGroup</span><span class="sxs-lookup"><span data-stu-id="308e9-101">Create sectionGroup</span></span>

<span data-ttu-id="308e9-102">Создание [группы разделов](../resources/sectiongroup.md) в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="308e9-102">Create a new [section group](../resources/sectiongroup.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="308e9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="308e9-103">Permissions</span></span>
<span data-ttu-id="308e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="308e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="308e9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="308e9-106">Permission type</span></span>      | <span data-ttu-id="308e9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="308e9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="308e9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="308e9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="308e9-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="308e9-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="308e9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="308e9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="308e9-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="308e9-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="308e9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="308e9-112">Application</span></span> | <span data-ttu-id="308e9-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="308e9-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="308e9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="308e9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
POST /groups/{id}/onenote/notebooks/{id}/sectionGroups
POST /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="308e9-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="308e9-115">Request headers</span></span>
| <span data-ttu-id="308e9-116">Имя</span><span class="sxs-lookup"><span data-stu-id="308e9-116">Name</span></span>       | <span data-ttu-id="308e9-117">Тип</span><span class="sxs-lookup"><span data-stu-id="308e9-117">Type</span></span> | <span data-ttu-id="308e9-118">Описание</span><span class="sxs-lookup"><span data-stu-id="308e9-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="308e9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="308e9-119">Authorization</span></span>  | <span data-ttu-id="308e9-120">string</span><span class="sxs-lookup"><span data-stu-id="308e9-120">string</span></span>  | <span data-ttu-id="308e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="308e9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="308e9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="308e9-123">Content-Type</span></span> | <span data-ttu-id="308e9-124">строка</span><span class="sxs-lookup"><span data-stu-id="308e9-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="308e9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="308e9-125">Request body</span></span>
<span data-ttu-id="308e9-126">В теле запроса укажите имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="308e9-126">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="308e9-p103">В рамках одного и того же уровня иерархии имя каждой группы разделов должно быть уникальным. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="308e9-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="308e9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="308e9-129">Response</span></span>

<span data-ttu-id="308e9-130">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="308e9-130">If successful, this method returns `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="308e9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="308e9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="308e9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="308e9-132">Request</span></span>
<span data-ttu-id="308e9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="308e9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```

##### <a name="response"></a><span data-ttu-id="308e9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="308e9-134">Response</span></span>
<span data-ttu-id="308e9-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="308e9-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
