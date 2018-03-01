# <a name="update-educationclass-properties"></a><span data-ttu-id="3b238-101">Обновление свойств educationclass</span><span class="sxs-lookup"><span data-stu-id="3b238-101">Update educationclass properties</span></span>

<span data-ttu-id="3b238-102">Обновление свойств курса.</span><span class="sxs-lookup"><span data-stu-id="3b238-102">Update the properties of a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b238-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b238-103">Permissions</span></span>
<span data-ttu-id="3b238-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3b238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b238-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b238-106">Permission type</span></span>      | <span data-ttu-id="3b238-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b238-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b238-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b238-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="3b238-109">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b238-109">Not supported.</span></span>  |
|<span data-ttu-id="3b238-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b238-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b238-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b238-111">Not supported.</span></span>   |
|<span data-ttu-id="3b238-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b238-112">Application</span></span> | <span data-ttu-id="3b238-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b238-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3b238-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b238-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3b238-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b238-115">Request headers</span></span>
| <span data-ttu-id="3b238-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b238-116">Header</span></span>       | <span data-ttu-id="3b238-117">Значение</span><span class="sxs-lookup"><span data-stu-id="3b238-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b238-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b238-118">Authorization</span></span>  | <span data-ttu-id="3b238-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b238-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3b238-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b238-121">Content-Type</span></span>  | <span data-ttu-id="3b238-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3b238-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b238-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b238-123">Request body</span></span>
<span data-ttu-id="3b238-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3b238-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3b238-125">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="3b238-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3b238-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3b238-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3b238-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b238-127">Property</span></span>     | <span data-ttu-id="3b238-128">Тип</span><span class="sxs-lookup"><span data-stu-id="3b238-128">Type</span></span>   |<span data-ttu-id="3b238-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3b238-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b238-130">description</span><span class="sxs-lookup"><span data-stu-id="3b238-130">description</span></span>|<span data-ttu-id="3b238-131">String</span><span class="sxs-lookup"><span data-stu-id="3b238-131">String</span></span>| <span data-ttu-id="3b238-132">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="3b238-132">Description of the template.</span></span>|
|<span data-ttu-id="3b238-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3b238-133">displayName</span></span>|<span data-ttu-id="3b238-134">String</span><span class="sxs-lookup"><span data-stu-id="3b238-134">String</span></span>| <span data-ttu-id="3b238-135">Название курса.</span><span class="sxs-lookup"><span data-stu-id="3b238-135">Name of the class.</span></span>|
|<span data-ttu-id="3b238-136">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3b238-136">mailNickname</span></span>|<span data-ttu-id="3b238-137">String</span><span class="sxs-lookup"><span data-stu-id="3b238-137">String</span></span>| <span data-ttu-id="3b238-138">Почтовый псевдоним для отправки электронных сообщений всем пользователям, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="3b238-138">Email alias for sending email to all users if that feature is enabled.</span></span> |
<!-- Please verify the revised description here. -->
<span data-ttu-id="3b238-139">Свойство classCode типа String представляет собой код курса, используемый учебным заведением. Свойство externalId типа String представляет собой идентификатор курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="3b238-139">|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="3b238-140">Свойство externalName типа String представляет собой название курса в системе синхронизации. Свойство externalSource типа String представляет собой способ создания курса.</span><span class="sxs-lookup"><span data-stu-id="3b238-140">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="3b238-141">Возможные значения: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="3b238-141">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>

## <a name="response"></a><span data-ttu-id="3b238-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b238-142">Response</span></span>
<span data-ttu-id="3b238-143">При успешном выполнении этот метод возвратит код отклика `200 OK` и обновленный объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3b238-143">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b238-144">Пример</span><span class="sxs-lookup"><span data-stu-id="3b238-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b238-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b238-145">Request</span></span>
<span data-ttu-id="3b238-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b238-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="3b238-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b238-147">Response</span></span>
<span data-ttu-id="3b238-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b238-148">The following is an example of the response.</span></span> 

><span data-ttu-id="3b238-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b238-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->