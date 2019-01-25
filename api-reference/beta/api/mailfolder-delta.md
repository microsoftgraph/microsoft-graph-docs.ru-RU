---
title: 'mailFolder: delta'
description: Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b4aac9c0370084cd0c5450e304737a11c93dd8f7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522604"
---
# <a name="mailfolder-delta"></a><span data-ttu-id="416a3-103">mailFolder: delta</span><span class="sxs-lookup"><span data-stu-id="416a3-103">mailFolder: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="416a3-104">Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.</span><span class="sxs-lookup"><span data-stu-id="416a3-104">Get a set of mail folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="416a3-p101">Вызов функции **delta** для почтовых папок в почтовом ящике похож на запрос GET, однако, правильно применяя [токены состояния](/graph/delta-query-overview) в этих вызовах, можно запрашивать изменения в папках почты. Это позволяет синхронизировать локальное хранилище почтовых папок пользователя, не загружая каждый раз все почтовые папки этого почтового ящика с сервера.</span><span class="sxs-lookup"><span data-stu-id="416a3-p101">A **delta** function call for mail folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the mail folders. This allows you to maintain and synchronize a local store of a user's mail folders without having to fetch all the mail folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="416a3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="416a3-107">Permissions</span></span>
<span data-ttu-id="416a3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="416a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="416a3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="416a3-110">Permission type</span></span>      | <span data-ttu-id="416a3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="416a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="416a3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="416a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="416a3-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="416a3-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="416a3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="416a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="416a3-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="416a3-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="416a3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="416a3-116">Application</span></span> | <span data-ttu-id="416a3-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="416a3-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="416a3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="416a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/delta
GET /users/<id>/mailFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="416a3-119">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="416a3-119">Query parameters</span></span>

<span data-ttu-id="416a3-p103">Отслеживание изменений в папках почты — это цикл из одного или нескольких вызовов функции **delta**. Если вы используете параметры запроса, отличные от `$deltatoken` и `$skiptoken`, их необходимо указать в первом запросе **delta**. Microsoft Graph автоматически кодирует указанные параметры в токене, входящем в состав URL-адреса `nextLink` или `deltaLink`, включенного в ответ. Параметры запроса нужно указать только один раз в первом запросе. Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="416a3-p103">Tracking changes in mail folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="416a3-125">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="416a3-125">Query parameter</span></span>      | <span data-ttu-id="416a3-126">Тип</span><span class="sxs-lookup"><span data-stu-id="416a3-126">Type</span></span>   |<span data-ttu-id="416a3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="416a3-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="416a3-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="416a3-128">$deltatoken</span></span> | <span data-ttu-id="416a3-129">string</span><span class="sxs-lookup"><span data-stu-id="416a3-129">string</span></span> | <span data-ttu-id="416a3-p104">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `deltaLink` предыдущего вызова функции **delta** для той же коллекции почтовых папок и указывает на завершение этого цикла отслеживания изменений. Сохраните URL-адрес `deltaLink` с этим токеном и примените его в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="416a3-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same mail folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="416a3-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="416a3-132">$skiptoken</span></span> | <span data-ttu-id="416a3-133">строка</span><span class="sxs-lookup"><span data-stu-id="416a3-133">string</span></span> | <span data-ttu-id="416a3-134">Этот [токен состояния](/graph/delta-query-overview) возвращается в URL-адресе `nextLink` предыдущего вызова функции **delta** и указывает, что из коллекции почтовых папок получены не все изменения.</span><span class="sxs-lookup"><span data-stu-id="416a3-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same mail folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="416a3-135">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="416a3-135">OData query parameters</span></span>

<span data-ttu-id="416a3-p105">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="416a3-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="416a3-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="416a3-138">Request headers</span></span>
| <span data-ttu-id="416a3-139">Имя</span><span class="sxs-lookup"><span data-stu-id="416a3-139">Name</span></span>       | <span data-ttu-id="416a3-140">Тип</span><span class="sxs-lookup"><span data-stu-id="416a3-140">Type</span></span> | <span data-ttu-id="416a3-141">Описание</span><span class="sxs-lookup"><span data-stu-id="416a3-141">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="416a3-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="416a3-142">Authorization</span></span>  | <span data-ttu-id="416a3-143">string</span><span class="sxs-lookup"><span data-stu-id="416a3-143">string</span></span>  | <span data-ttu-id="416a3-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="416a3-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="416a3-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="416a3-146">Content-Type</span></span>  | <span data-ttu-id="416a3-147">string</span><span class="sxs-lookup"><span data-stu-id="416a3-147">string</span></span>  | <span data-ttu-id="416a3-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="416a3-p107">application/json. Required.</span></span> |
| <span data-ttu-id="416a3-150">Prefer</span><span class="sxs-lookup"><span data-stu-id="416a3-150">Prefer</span></span> | <span data-ttu-id="416a3-151">string</span><span class="sxs-lookup"><span data-stu-id="416a3-151">string</span></span>  | <span data-ttu-id="416a3-p108">odata.maxpagesize={x}. Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="416a3-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="416a3-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="416a3-154">Response</span></span>

<span data-ttu-id="416a3-155">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект коллекции [mailFolder](../resources/mailfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="416a3-155">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="416a3-156">Пример</span><span class="sxs-lookup"><span data-stu-id="416a3-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="416a3-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="416a3-157">Request</span></span>
<span data-ttu-id="416a3-158">В следующем примере показано, как выполнить один вызов функции **delta** и ограничить максимальное количество папок почты в тексте ответа до 2.</span><span class="sxs-lookup"><span data-stu-id="416a3-158">The following example shows how to make a single **delta** function call, and limit the maximum number of mail folders in the response body to 2.</span></span>

<span data-ttu-id="416a3-159">Чтобы отследить изменения в почтовых папках почтового ящика, выполните один или несколько вызовов функции **delta** с правильными токенами состояния, чтобы получить набор изменений с момента последнего запроса.</span><span class="sxs-lookup"><span data-stu-id="416a3-159">To track changes in the mail folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="416a3-p109">Пример, в котором показано, как использовать токены состояния для отслеживания изменений в сообщениях почтовой папки: [Получение добавочных изменений для сообщений в папке](/graph/delta-query-messages). Отслеживание почтовых папок и отслеживание сообщений в папке отличаются URL-адресами запроса изменений и тем, что в ответах возвращаются коллекции **mailFolder**, а не **message**.</span><span class="sxs-lookup"><span data-stu-id="416a3-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking mail folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **mailFolder** rather than **message** collections.</span></span>

<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="416a3-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="416a3-162">Response</span></span>

<span data-ttu-id="416a3-163">В случае успешного выполнения запроса отклик будет содержать маркер состояния — _skipToken_</span><span class="sxs-lookup"><span data-stu-id="416a3-163">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="416a3-p110">или _deltaToken_. Первый включен в заголовок отклика _@odata.nextLink_, второй — в заголовок отклика _@odata.deltaLink_. Первый указывает на необходимость продолжать цикл, второй — на наличие всех изменений для определенного цикла.</span><span class="sxs-lookup"><span data-stu-id="416a3-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="416a3-166">Ниже показан отклик с маркером состояния _skipToken_ в заголовке отклика _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="416a3-166">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="416a3-p111">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="416a3-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="see-also"></a><span data-ttu-id="416a3-169">См. также</span><span class="sxs-lookup"><span data-stu-id="416a3-169">See also</span></span>

- [<span data-ttu-id="416a3-170">Запрос изменений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="416a3-170">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="416a3-171">Получение добавочных изменений сообщений в папке</span><span class="sxs-lookup"><span data-stu-id="416a3-171">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

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
    "Error: /api-reference/beta/api/mailfolder-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
