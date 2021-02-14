---
title: Удаление участника
description: Удаление определенного участника в вызове.
manager: zhengni
author: jackry6350
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 40171c4cea7fe97fb20dc7ef3bfb7e27ff287bf3
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240390"
---
# <a name="delete-participant"></a><span data-ttu-id="c7afe-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="c7afe-103">Delete participant</span></span>

<span data-ttu-id="c7afe-104">Удаление определенного участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="c7afe-104">Delete a specific participant in a call.</span></span> <span data-ttu-id="c7afe-105">В некоторых ситуациях приложение может удалить участника из активного вызова.</span><span class="sxs-lookup"><span data-stu-id="c7afe-105">In some situations, it is appropriate for an application to remove a participant from an active call.</span></span> <span data-ttu-id="c7afe-106">Это действие можно сделать после того, как участник ответит на вызов.</span><span class="sxs-lookup"><span data-stu-id="c7afe-106">This action can be done after the participant answers the call.</span></span> <span data-ttu-id="c7afe-107">При удалении активного вызываемого, он немедленно удаляется из звонка без предварительного или после удаления уведомления.</span><span class="sxs-lookup"><span data-stu-id="c7afe-107">When an active caller is removed, they are immediately dropped from the call with no pre- or post-removal notification.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7afe-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7afe-108">Permissions</span></span>
<span data-ttu-id="c7afe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7afe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7afe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7afe-111">Permission type</span></span>                        | <span data-ttu-id="c7afe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7afe-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c7afe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7afe-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7afe-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7afe-114">Not Supported</span></span>                               |
| <span data-ttu-id="c7afe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7afe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7afe-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7afe-116">Not Supported</span></span>                               |
| <span data-ttu-id="c7afe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7afe-117">Application</span></span>                            | <span data-ttu-id="c7afe-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c7afe-118">None</span></span>                                        |

<span data-ttu-id="c7afe-119">Чтобы разрешить приложению вызывать этот API, необходима конфигурация собрания на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="c7afe-119">Tenant-level application meeting configuration is required to allow an application to call this API.</span></span> <span data-ttu-id="c7afe-120">Администратор клиента должен вызвать следующий cmdlet в удаленной powerShell клиента, чтобы предоставить приложению разрешение на вызов этого API.</span><span class="sxs-lookup"><span data-stu-id="c7afe-120">The tenant admin should call the following cmdlet on the tenant remote PowerShell to grant the permission to the application to call this API.</span></span> <span data-ttu-id="c7afe-121">Дополнительные сведения [см. в подстроке Set-CsApplicationMeetingConfiguration.](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c7afe-121">For more information, see [Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span></span>
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a><span data-ttu-id="c7afe-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7afe-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}/participants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c7afe-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7afe-123">Request headers</span></span>
| <span data-ttu-id="c7afe-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c7afe-124">Name</span></span>          | <span data-ttu-id="c7afe-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c7afe-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c7afe-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7afe-126">Authorization</span></span> | <span data-ttu-id="c7afe-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7afe-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7afe-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7afe-129">Request body</span></span>
<span data-ttu-id="c7afe-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7afe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7afe-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7afe-131">Response</span></span>
<span data-ttu-id="c7afe-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c7afe-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7afe-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c7afe-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c7afe-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7afe-135">Request</span></span>
<span data-ttu-id="c7afe-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7afe-136">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7afe-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7afe-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/{id}/participants/{id}
```
# <a name="c"></a>[<span data-ttu-id="c7afe-138">C#</span><span class="sxs-lookup"><span data-stu-id="c7afe-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7afe-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7afe-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7afe-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7afe-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7afe-141">Java</span><span class="sxs-lookup"><span data-stu-id="c7afe-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c7afe-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7afe-142">Response</span></span>

> <span data-ttu-id="c7afe-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7afe-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
