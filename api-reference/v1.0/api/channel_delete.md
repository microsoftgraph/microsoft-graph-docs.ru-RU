# <a name="delete-channel"></a><span data-ttu-id="e5ec5-101">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="e5ec5-101">Delete channel</span></span>



<span data-ttu-id="e5ec5-102">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="e5ec5-102">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="e5ec5-103">**Примечание**: существует известная проблема с разрешениями приложения и этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="e5ec5-103">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="e5ec5-104">Дополнительные сведения см [Известные проблемы списка](../../../concepts/known_issues.md#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="e5ec5-104">For details, see the [known issues list](../../../concepts/known_issues.md#application-permissions).</span></span>

> <span data-ttu-id="e5ec5-105">**Примечание**: данных в удаленные каналы будут храниться в течение нескольких недель разрешить владельцем группы для восстановления удаленных канала.</span><span class="sxs-lookup"><span data-stu-id="e5ec5-105">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="e5ec5-106">В это время новый канал с одной displayName может быть создан.</span><span class="sxs-lookup"><span data-stu-id="e5ec5-106">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5ec5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5ec5-107">Permissions</span></span>
<span data-ttu-id="e5ec5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e5ec5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e5ec5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5ec5-110">Permission type</span></span>      | <span data-ttu-id="e5ec5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5ec5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5ec5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5ec5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e5ec5-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5ec5-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5ec5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5ec5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5ec5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ec5-115">Not supported.</span></span>    |
|<span data-ttu-id="e5ec5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5ec5-116">Application</span></span> | <span data-ttu-id="e5ec5-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5ec5-117">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="e5ec5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5ec5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e5ec5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5ec5-119">Request headers</span></span>
| <span data-ttu-id="e5ec5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5ec5-120">Header</span></span>       | <span data-ttu-id="e5ec5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5ec5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5ec5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5ec5-122">Authorization</span></span>  | <span data-ttu-id="e5ec5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5ec5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5ec5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5ec5-125">Request body</span></span>
<span data-ttu-id="e5ec5-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5ec5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5ec5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5ec5-127">Response</span></span>

<span data-ttu-id="e5ec5-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e5ec5-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5ec5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e5ec5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5ec5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5ec5-131">Request</span></span>
<span data-ttu-id="e5ec5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5ec5-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="e5ec5-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5ec5-133">Response</span></span>

<span data-ttu-id="e5ec5-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e5ec5-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
