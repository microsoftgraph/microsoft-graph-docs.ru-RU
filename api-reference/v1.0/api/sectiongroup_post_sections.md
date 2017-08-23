# <a name="create-section"></a><span data-ttu-id="7d897-101">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="7d897-101">Create section</span></span>

<span data-ttu-id="7d897-102">Создание объекта [section](../resources/section.md) в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="7d897-102">Create a new [section](../resources/section.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d897-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d897-103">Permissions</span></span>
<span data-ttu-id="7d897-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7d897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7d897-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d897-106">Permission type</span></span>      | <span data-ttu-id="7d897-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d897-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="7d897-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d897-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7d897-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d897-109">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="7d897-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d897-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d897-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d897-111">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="7d897-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d897-112">Application</span></span> | <span data-ttu-id="7d897-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d897-113">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7d897-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d897-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="7d897-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d897-115">Request headers</span></span>
| <span data-ttu-id="7d897-116">Имя</span><span class="sxs-lookup"><span data-stu-id="7d897-116">Name</span></span>       | <span data-ttu-id="7d897-117">Тип</span><span class="sxs-lookup"><span data-stu-id="7d897-117">Type</span></span> | <span data-ttu-id="7d897-118">Описание</span><span class="sxs-lookup"><span data-stu-id="7d897-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d897-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d897-119">Authorization</span></span>  | <span data-ttu-id="7d897-120">string</span><span class="sxs-lookup"><span data-stu-id="7d897-120">string</span></span>  | <span data-ttu-id="7d897-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d897-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d897-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d897-123">Content-Type</span></span> | <span data-ttu-id="7d897-124">строка</span><span class="sxs-lookup"><span data-stu-id="7d897-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7d897-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d897-125">Request body</span></span>
<span data-ttu-id="7d897-126">В тексте запроса укажите имя раздела.</span><span class="sxs-lookup"><span data-stu-id="7d897-126">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="7d897-p103">В рамках одного и того же уровня иерархии имена разделов должны быть уникальными. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="7d897-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="7d897-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d897-129">Response</span></span>

<span data-ttu-id="7d897-130">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [section](../resources/section.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7d897-130">If successful, this method returns a `201 Created` response code and a [section](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d897-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7d897-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d897-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d897-132">Request</span></span>
<span data-ttu-id="7d897-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d897-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```

##### <a name="response"></a><span data-ttu-id="7d897-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d897-134">Response</span></span>
<span data-ttu-id="7d897-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d897-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
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
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->