# <a name="create-section"></a><span data-ttu-id="e9dde-101">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="e9dde-101">Create section</span></span>

<span data-ttu-id="e9dde-102">Создание нового раздела [onenoteSection](../resources/section.md) в указанной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="e9dde-102">Create a new [section](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9dde-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9dde-103">Permissions</span></span>
<span data-ttu-id="e9dde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9dde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e9dde-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9dde-106">Permission type</span></span>      | <span data-ttu-id="e9dde-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9dde-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9dde-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9dde-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e9dde-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9dde-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9dde-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9dde-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9dde-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9dde-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e9dde-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9dde-112">Application</span></span> | <span data-ttu-id="e9dde-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9dde-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9dde-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9dde-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="e9dde-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9dde-115">Request headers</span></span>
| <span data-ttu-id="e9dde-116">Имя</span><span class="sxs-lookup"><span data-stu-id="e9dde-116">Name</span></span>       | <span data-ttu-id="e9dde-117">Тип</span><span class="sxs-lookup"><span data-stu-id="e9dde-117">Type</span></span> | <span data-ttu-id="e9dde-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e9dde-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9dde-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9dde-119">Authorization</span></span>  | <span data-ttu-id="e9dde-120">строка</span><span class="sxs-lookup"><span data-stu-id="e9dde-120">string</span></span>  | <span data-ttu-id="e9dde-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9dde-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9dde-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9dde-123">Content-Type</span></span> | <span data-ttu-id="e9dde-124">string</span><span class="sxs-lookup"><span data-stu-id="e9dde-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e9dde-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9dde-125">Request body</span></span>
<span data-ttu-id="e9dde-126">В тексте запроса укажите имя раздела.</span><span class="sxs-lookup"><span data-stu-id="e9dde-126">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="e9dde-p103">В рамках одного и того же уровня иерархии имена разделов должны быть уникальными. Имя должно содержать не более 50 символов, в нем не должно быть следующих знаков:  ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="e9dde-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="e9dde-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9dde-129">Response</span></span>

<span data-ttu-id="e9dde-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [onenoteSection](../resources/section.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9dde-130">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9dde-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e9dde-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9dde-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9dde-132">Request</span></span>
<span data-ttu-id="e9dde-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9dde-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="e9dde-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9dde-134">Response</span></span>
<span data-ttu-id="e9dde-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9dde-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 201 Created
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
