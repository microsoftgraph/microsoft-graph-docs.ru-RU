# <a name="group-subscribebymail"></a><span data-ttu-id="84008-101">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="84008-101">group: subscribeByMail</span></span>

<span data-ttu-id="84008-p101">С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="84008-p101">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="84008-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84008-104">Permissions</span></span>
<span data-ttu-id="84008-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="84008-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="84008-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84008-107">Permission type</span></span>      | <span data-ttu-id="84008-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84008-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84008-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84008-109">Delegated (work or school account)</span></span> | <span data-ttu-id="84008-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84008-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="84008-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84008-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84008-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84008-112">Not supported.</span></span>    |
|<span data-ttu-id="84008-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84008-113">Application</span></span> | <span data-ttu-id="84008-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84008-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84008-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84008-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="84008-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84008-116">Request headers</span></span>
| <span data-ttu-id="84008-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84008-117">Header</span></span>       | <span data-ttu-id="84008-118">Значение</span><span class="sxs-lookup"><span data-stu-id="84008-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="84008-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84008-119">Authorization</span></span>  | <span data-ttu-id="84008-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84008-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84008-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84008-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="84008-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="84008-123">Response</span></span>
<span data-ttu-id="84008-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="84008-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84008-126">Пример</span><span class="sxs-lookup"><span data-stu-id="84008-126">Example</span></span>
<span data-ttu-id="84008-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="84008-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="84008-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="84008-128">Request</span></span>
<span data-ttu-id="84008-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84008-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

##### <a name="response"></a><span data-ttu-id="84008-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="84008-130">Response</span></span>
<span data-ttu-id="84008-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="84008-131">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->