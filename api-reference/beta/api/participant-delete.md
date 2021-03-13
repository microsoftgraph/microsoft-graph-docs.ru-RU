---
title: Удаление участника
description: Удаление определенного участника в вызове.
manager: zhengni
author: jackry6350
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 3fd701f9fb346a86c93359cdaa1a360c9b484223
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50769364"
---
# <a name="delete-participant"></a><span data-ttu-id="e1633-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="e1633-103">Delete participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1633-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1633-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1633-105">Удаление определенного участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="e1633-105">Delete a specific participant in a call.</span></span> <span data-ttu-id="e1633-106">В некоторых ситуациях приложение может удалить участника из активного вызова.</span><span class="sxs-lookup"><span data-stu-id="e1633-106">In some situations, it is appropriate for an application to remove a participant from an active call.</span></span> <span data-ttu-id="e1633-107">Это действие можно сделать после ответа участника на вызов.</span><span class="sxs-lookup"><span data-stu-id="e1633-107">This action can be done after the participant answers the call.</span></span> <span data-ttu-id="e1633-108">При удалении активного вызываемого звонка он немедленно удаляется из вызова без предварительного или после удаления уведомления.</span><span class="sxs-lookup"><span data-stu-id="e1633-108">When an active caller is removed, they are immediately dropped from the call with no pre- or post-removal notification.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1633-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1633-109">Permissions</span></span>
<span data-ttu-id="e1633-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1633-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1633-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1633-112">Permission type</span></span>                        | <span data-ttu-id="e1633-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1633-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e1633-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1633-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1633-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e1633-115">Not Supported</span></span>                               |
| <span data-ttu-id="e1633-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1633-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1633-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e1633-117">Not Supported</span></span>                               |
| <span data-ttu-id="e1633-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1633-118">Application</span></span>                            | <span data-ttu-id="e1633-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e1633-119">None</span></span>                                        |

<span data-ttu-id="e1633-120">Конфигурация собрания на уровне клиента требуется для того, чтобы позволить приложению вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e1633-120">Tenant-level application meeting configuration is required to allow an application to call this API.</span></span> <span data-ttu-id="e1633-121">Администратор клиента должен вызвать следующий комдлет на удаленной PowerShell клиента, чтобы предоставить приложению разрешение на вызов этого API.</span><span class="sxs-lookup"><span data-stu-id="e1633-121">The tenant admin should call the following cmdlet on the tenant remote PowerShell to grant the permission to the application to call this API.</span></span> <span data-ttu-id="e1633-122">Дополнительные сведения см. [в рублях Set-CsApplicationMeetingConfiguration.](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1633-122">For more information, see [Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span></span>
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a><span data-ttu-id="e1633-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1633-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/participants/{id}
DELETE /communications/calls/{id}/participants/{id}
```
> <span data-ttu-id="e1633-124">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="e1633-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e1633-125">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e1633-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1633-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1633-126">Request headers</span></span>
| <span data-ttu-id="e1633-127">Имя</span><span class="sxs-lookup"><span data-stu-id="e1633-127">Name</span></span>          | <span data-ttu-id="e1633-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e1633-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e1633-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1633-129">Authorization</span></span> | <span data-ttu-id="e1633-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1633-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1633-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1633-132">Request body</span></span>
<span data-ttu-id="e1633-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1633-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1633-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1633-134">Response</span></span>
<span data-ttu-id="e1633-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1633-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1633-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e1633-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1633-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1633-138">Request</span></span>
<span data-ttu-id="e1633-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1633-139">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1633-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1633-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/participants/{id}
```
# <a name="c"></a>[<span data-ttu-id="e1633-141">C#</span><span class="sxs-lookup"><span data-stu-id="e1633-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1633-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1633-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1633-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1633-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1633-144">Java</span><span class="sxs-lookup"><span data-stu-id="e1633-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1633-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1633-145">Response</span></span>

> <span data-ttu-id="e1633-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1633-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Delete participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
