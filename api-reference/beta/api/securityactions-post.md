---
title: Создание объекта securityAction
description: Создайте новый объект securityAction. "
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c8f9e98e57a351bd17776c77449f7d1ff8d8a897
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482016"
---
# <a name="create-securityaction"></a><span data-ttu-id="b1611-103">Создание объекта securityAction</span><span class="sxs-lookup"><span data-stu-id="b1611-103">Create securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1611-104">Создайте новый объект [securityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="b1611-104">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1611-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1611-105">Permissions</span></span>

<span data-ttu-id="b1611-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1611-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1611-108">Permission type</span></span>                        | <span data-ttu-id="b1611-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1611-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b1611-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1611-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1611-111">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1611-111">SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="b1611-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1611-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1611-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1611-113">Not supported.</span></span> |
| <span data-ttu-id="b1611-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1611-114">Application</span></span>                            | <span data-ttu-id="b1611-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1611-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1611-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1611-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="b1611-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1611-117">Request headers</span></span>

| <span data-ttu-id="b1611-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b1611-118">Name</span></span>          | <span data-ttu-id="b1611-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b1611-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b1611-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1611-120">Authorization</span></span> | <span data-ttu-id="b1611-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b1611-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1611-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1611-122">Request body</span></span>

<span data-ttu-id="b1611-123">В тексте запроса добавьте представление объекта [securityAction](../resources/securityaction.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1611-123">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b1611-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1611-124">Response</span></span>

<span data-ttu-id="b1611-125">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [securityAction](../resources/securityaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1611-125">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1611-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="b1611-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1611-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1611-127">Request</span></span>

<span data-ttu-id="b1611-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1611-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_securityaction_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions
Content-type: application/json

{
  "name": "BlockIp",
  "actionReason": "Test",
  "parameters": [
    {
      "name": "IP",
      "value": "1.2.3.4"
    }
  ],
  "vendorInformation": {
    "provider": "Windows Defender ATP",
    "vendor": "Microsoft"
  }
}
```

### <a name="response"></a><span data-ttu-id="b1611-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1611-129">Response</span></span>

<span data-ttu-id="b1611-130">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1611-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b1611-131">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b1611-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b1611-132">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1611-132">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id" : "1234567890",
    "status" : "notStarted",
    "createdDateTime": "2019-01-10 12:23:23.33333",
    "lastActionDateTime": "2019-01-10 12:23:23.33333",
    "name": "blockIp",
    "actionReason": "Test",
    "errorInfo": null,
    "vendorInformation": {
        "provider": "Windows Defender ATP",
        "providerVersion": null,
        "subProvider": null,
        "vendor": "Microsoft"
    },
    "parameters": [
        {
            "name": "IP",
            "value": "1.2.3.4"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
