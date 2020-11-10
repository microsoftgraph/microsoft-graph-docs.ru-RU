---
title: 'mailFolder: delta'
description: Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 384c340f5cb89772ade4e264237d34fde00e4881
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979396"
---
# <a name="mailfolder-delta"></a><span data-ttu-id="003b1-103">mailFolder: delta</span><span class="sxs-lookup"><span data-stu-id="003b1-103">mailFolder: delta</span></span>

<span data-ttu-id="003b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="003b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="003b1-105">Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="003b1-105">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="003b1-p101">Вызов функции **delta** для почтовых папок в почтовом ящике похож на запрос GET, однако, правильно применяя [токены состояния](/graph/delta-query-overview) в этих вызовах, можно запрашивать изменения в папках почты. Это позволяет синхронизировать локальное хранилище почтовых папок пользователя, не загружая каждый раз все почтовые папки этого почтового ящика с сервера.</span><span class="sxs-lookup"><span data-stu-id="003b1-p101">A **delta** function call for mail folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the mail folders. This allows you to maintain and synchronize a local store of a user's mail folders without having to fetch all the mail folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="003b1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="003b1-108">Permissions</span></span>
<span data-ttu-id="003b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="003b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="003b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="003b1-111">Permission type</span></span>      | <span data-ttu-id="003b1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="003b1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="003b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="003b1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="003b1-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003b1-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="003b1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="003b1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="003b1-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003b1-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="003b1-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="003b1-117">Application</span></span> | <span data-ttu-id="003b1-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003b1-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="003b1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="003b1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/delta
GET /users/{id}/mailFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="003b1-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="003b1-120">Query parameters</span></span>

<span data-ttu-id="003b1-p103">Отслеживание изменений в папках почты — это цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в первом запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в ответ. Параметры запроса нужно указать только один раз в первом запросе. Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="003b1-p103">Tracking changes in mail folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="003b1-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="003b1-126">Query parameter</span></span>      | <span data-ttu-id="003b1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="003b1-127">Type</span></span>   |<span data-ttu-id="003b1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="003b1-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="003b1-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="003b1-129">$deltatoken</span></span> | <span data-ttu-id="003b1-130">string</span><span class="sxs-lookup"><span data-stu-id="003b1-130">string</span></span> | <span data-ttu-id="003b1-p104">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции почтовых папок и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="003b1-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same mail folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="003b1-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="003b1-133">$skiptoken</span></span> | <span data-ttu-id="003b1-134">string</span><span class="sxs-lookup"><span data-stu-id="003b1-134">string</span></span> | <span data-ttu-id="003b1-135">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции почтовых папок получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="003b1-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same mail folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="003b1-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="003b1-136">OData query parameters</span></span>

<span data-ttu-id="003b1-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="003b1-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="003b1-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="003b1-139">Request headers</span></span>
| <span data-ttu-id="003b1-140">Имя</span><span class="sxs-lookup"><span data-stu-id="003b1-140">Name</span></span>       | <span data-ttu-id="003b1-141">Тип</span><span class="sxs-lookup"><span data-stu-id="003b1-141">Type</span></span> | <span data-ttu-id="003b1-142">Описание</span><span class="sxs-lookup"><span data-stu-id="003b1-142">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="003b1-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="003b1-143">Authorization</span></span>  | <span data-ttu-id="003b1-144">string</span><span class="sxs-lookup"><span data-stu-id="003b1-144">string</span></span>  | <span data-ttu-id="003b1-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="003b1-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="003b1-147">Content-Type</span><span class="sxs-lookup"><span data-stu-id="003b1-147">Content-Type</span></span>  | <span data-ttu-id="003b1-148">string</span><span class="sxs-lookup"><span data-stu-id="003b1-148">string</span></span>  | <span data-ttu-id="003b1-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="003b1-p107">application/json. Required.</span></span> |
| <span data-ttu-id="003b1-151">Prefer</span><span class="sxs-lookup"><span data-stu-id="003b1-151">Prefer</span></span> | <span data-ttu-id="003b1-152">string</span><span class="sxs-lookup"><span data-stu-id="003b1-152">string</span></span>  | <span data-ttu-id="003b1-p108">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="003b1-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="003b1-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="003b1-155">Response</span></span>

<span data-ttu-id="003b1-156">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект коллекции [mailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="003b1-156">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="003b1-157">Пример</span><span class="sxs-lookup"><span data-stu-id="003b1-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="003b1-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="003b1-158">Request</span></span>
<span data-ttu-id="003b1-159">В следующем примере показано, как выполнить один вызов функции **delta** и ограничить максимальное количество папок почты в тексте ответа до 2.</span><span class="sxs-lookup"><span data-stu-id="003b1-159">The following example shows how to make a single **delta** function call, and limit the maximum number of mail folders in the response body to 2.</span></span>

<span data-ttu-id="003b1-160">Чтобы отследить изменения в почтовых папках почтового ящика, выполните один или несколько вызовов функции **delta** с правильными токенами состояния, чтобы получить набор изменений с момента последнего запроса.</span><span class="sxs-lookup"><span data-stu-id="003b1-160">To track changes in the mail folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="003b1-p109">Пример, в котором показано, как использовать токены состояния для отслеживания изменений в сообщениях почтовой папки: [Получение добавочных изменений для сообщений в папке](/graph/delta-query-messages). Отслеживание почтовых папок и отслеживание сообщений в папке отличаются URL-адресами запроса изменений и тем, что в ответах возвращаются коллекции **mailFolder** , а не **message**.</span><span class="sxs-lookup"><span data-stu-id="003b1-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking mail folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **mailFolder** rather than **message** collections.</span></span>


# <a name="http"></a>[<span data-ttu-id="003b1-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="003b1-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="003b1-164">C#</span><span class="sxs-lookup"><span data-stu-id="003b1-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="003b1-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="003b1-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="003b1-166">Java</span><span class="sxs-lookup"><span data-stu-id="003b1-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="003b1-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="003b1-167">Response</span></span>

<span data-ttu-id="003b1-168">В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_</span><span class="sxs-lookup"><span data-stu-id="003b1-168">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="003b1-p110">или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_ , второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.</span><span class="sxs-lookup"><span data-stu-id="003b1-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="003b1-171">Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="003b1-171">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="003b1-p111">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="003b1-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "wellKnownName": "wellKnownName-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="003b1-174">См. также</span><span class="sxs-lookup"><span data-stu-id="003b1-174">See also</span></span>

- [<span data-ttu-id="003b1-175">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="003b1-175">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="003b1-176">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="003b1-176">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


