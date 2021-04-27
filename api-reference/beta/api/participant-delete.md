---
title: Удаление участника
description: Удаление определенного участника в вызове.
manager: zhengni
author: jackry6350
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1ee50cd399b974b80fcb80ad514bbf3423c0471e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037876"
---
# <a name="delete-participant"></a><span data-ttu-id="31e4a-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="31e4a-103">Delete participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31e4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31e4a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31e4a-105">Удаление определенного участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="31e4a-105">Delete a specific participant in a call.</span></span> <span data-ttu-id="31e4a-106">В некоторых ситуациях приложение может удалить участника из активного вызова.</span><span class="sxs-lookup"><span data-stu-id="31e4a-106">In some situations, it is appropriate for an application to remove a participant from an active call.</span></span> <span data-ttu-id="31e4a-107">Это действие можно сделать после ответа участника на вызов.</span><span class="sxs-lookup"><span data-stu-id="31e4a-107">This action can be done after the participant answers the call.</span></span> <span data-ttu-id="31e4a-108">При удалении активного вызываемого звонка он немедленно удаляется из вызова без предварительного или после удаления уведомления.</span><span class="sxs-lookup"><span data-stu-id="31e4a-108">When an active caller is removed, they are immediately dropped from the call with no pre- or post-removal notification.</span></span>

## <a name="permissions"></a><span data-ttu-id="31e4a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31e4a-109">Permissions</span></span>
<span data-ttu-id="31e4a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31e4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31e4a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31e4a-112">Permission type</span></span>                        | <span data-ttu-id="31e4a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31e4a-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="31e4a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31e4a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="31e4a-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31e4a-115">Not Supported</span></span>                               |
| <span data-ttu-id="31e4a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31e4a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31e4a-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31e4a-117">Not Supported</span></span>                               |
| <span data-ttu-id="31e4a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31e4a-118">Application</span></span>                            | <span data-ttu-id="31e4a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="31e4a-119">None</span></span>                                        |

<span data-ttu-id="31e4a-120">Конфигурация собрания на уровне клиента требуется для того, чтобы позволить приложению вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="31e4a-120">Tenant-level application meeting configuration is required to allow an application to call this API.</span></span> <span data-ttu-id="31e4a-121">Администратор клиента должен вызвать следующий комдлет на удаленной PowerShell клиента, чтобы предоставить приложению разрешение на вызов этого API.</span><span class="sxs-lookup"><span data-stu-id="31e4a-121">The tenant admin should call the following cmdlet on the tenant remote PowerShell to grant the permission to the application to call this API.</span></span> <span data-ttu-id="31e4a-122">Дополнительные сведения см. [в рублях Set-CsApplicationMeetingConfiguration.](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31e4a-122">For more information, see [Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span></span>
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a><span data-ttu-id="31e4a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31e4a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/participants/{id}
DELETE /communications/calls/{id}/participants/{id}
```
> <span data-ttu-id="31e4a-124">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="31e4a-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="31e4a-125">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="31e4a-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31e4a-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31e4a-126">Request headers</span></span>
| <span data-ttu-id="31e4a-127">Имя</span><span class="sxs-lookup"><span data-stu-id="31e4a-127">Name</span></span>          | <span data-ttu-id="31e4a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="31e4a-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="31e4a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31e4a-129">Authorization</span></span> | <span data-ttu-id="31e4a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31e4a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31e4a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31e4a-132">Request body</span></span>
<span data-ttu-id="31e4a-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31e4a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31e4a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="31e4a-134">Response</span></span>
<span data-ttu-id="31e4a-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="31e4a-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31e4a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="31e4a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="31e4a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="31e4a-138">Request</span></span>
<span data-ttu-id="31e4a-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31e4a-139">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31e4a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="31e4a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/participants/{id}
```
# <a name="c"></a>[<span data-ttu-id="31e4a-141">C#</span><span class="sxs-lookup"><span data-stu-id="31e4a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31e4a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31e4a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31e4a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31e4a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31e4a-144">Java</span><span class="sxs-lookup"><span data-stu-id="31e4a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31e4a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="31e4a-145">Response</span></span>

> <span data-ttu-id="31e4a-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="31e4a-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
