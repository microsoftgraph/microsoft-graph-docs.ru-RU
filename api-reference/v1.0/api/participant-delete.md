---
title: Удаление участника
description: Удаление определенного участника в вызове.
manager: zhengni
author: jackry6350
ms.author: yoren
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8c08821f723152adb82cde0255d21ea3d8718a8e
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137160"
---
# <a name="delete-participant"></a><span data-ttu-id="293f6-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="293f6-103">Delete participant</span></span>

<span data-ttu-id="293f6-104">Удаление определенного участника в вызове.</span><span class="sxs-lookup"><span data-stu-id="293f6-104">Delete a specific participant in a call.</span></span> <span data-ttu-id="293f6-105">В некоторых ситуациях приложение может удалить участника из активного вызова.</span><span class="sxs-lookup"><span data-stu-id="293f6-105">In some situations, it is appropriate for an application to remove a participant from an active call.</span></span> <span data-ttu-id="293f6-106">Это действие можно выполнить как до, так и после того, как участник ответит на звонок.</span><span class="sxs-lookup"><span data-stu-id="293f6-106">This action can be done either before or after the participant answers the call.</span></span> <span data-ttu-id="293f6-107">После удаления активного вызывающего абонента он сразу же удаляется из вызова без уведомления о допуске или после удаления.</span><span class="sxs-lookup"><span data-stu-id="293f6-107">When an active caller is removed, they are immediately dropped from the call with no pre- or post-removal notification.</span></span>

## <a name="permissions"></a><span data-ttu-id="293f6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="293f6-108">Permissions</span></span>
<span data-ttu-id="293f6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="293f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="293f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="293f6-111">Permission type</span></span>                        | <span data-ttu-id="293f6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="293f6-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="293f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="293f6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="293f6-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="293f6-114">Not Supported</span></span>                               |
| <span data-ttu-id="293f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="293f6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="293f6-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="293f6-116">Not Supported</span></span>                               |
| <span data-ttu-id="293f6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="293f6-117">Application</span></span>                            | <span data-ttu-id="293f6-118">Нет</span><span class="sxs-lookup"><span data-stu-id="293f6-118">None</span></span>                                        |

<span data-ttu-id="293f6-119">Настройка собраний для приложения на уровне клиента необходима для того, чтобы приложение мог вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="293f6-119">Tenant-level application meeting configuration is required to allow an application to call this API.</span></span> <span data-ttu-id="293f6-120">Администратор клиента должен вызвать следующий командлет в удаленной оболочке PowerShell клиента, чтобы предоставить приложению разрешение на вызов этого API.</span><span class="sxs-lookup"><span data-stu-id="293f6-120">The tenant admin should call the following cmdlet on the tenant remote PowerShell to grant the permission to the application to call this API.</span></span> <span data-ttu-id="293f6-121">Дополнительные сведения см. в статье [Set – ксаппликатионмитингконфигуратион](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f6-121">For more information, see [Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span></span>
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a><span data-ttu-id="293f6-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="293f6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}/participants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="293f6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="293f6-123">Request headers</span></span>
| <span data-ttu-id="293f6-124">Имя</span><span class="sxs-lookup"><span data-stu-id="293f6-124">Name</span></span>          | <span data-ttu-id="293f6-125">Описание</span><span class="sxs-lookup"><span data-stu-id="293f6-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="293f6-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="293f6-126">Authorization</span></span> | <span data-ttu-id="293f6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="293f6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="293f6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="293f6-129">Request body</span></span>
<span data-ttu-id="293f6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="293f6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="293f6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="293f6-131">Response</span></span>
<span data-ttu-id="293f6-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="293f6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="293f6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="293f6-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="293f6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="293f6-135">Request</span></span>
<span data-ttu-id="293f6-136">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="293f6-136">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="293f6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="293f6-137">Response</span></span>

> <span data-ttu-id="293f6-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="293f6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
