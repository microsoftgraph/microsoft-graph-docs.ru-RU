---
title: Список существующих шаблонов синхронизации
description: Список шаблонов синхронизации, связанных с конкретным приложением или участником службы.
localization_priority: Normal
ms.openlocfilehash: 385d7b34c3efd1c7236b7d57dc1239acb328421e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330274"
---
# <a name="list-existing-synchronization-templates"></a><span data-ttu-id="a1086-103">Список существующих шаблонов синхронизации</span><span class="sxs-lookup"><span data-stu-id="a1086-103">List existing synchronization templates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1086-104">Список шаблонов синхронизации, связанных с конкретным приложением или участником службы.</span><span class="sxs-lookup"><span data-stu-id="a1086-104">List the synchronization templates associated with a given application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1086-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1086-105">Permissions</span></span>
<span data-ttu-id="a1086-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1086-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1086-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1086-108">Permission type</span></span>                        | <span data-ttu-id="a1086-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1086-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1086-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1086-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="a1086-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1086-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a1086-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1086-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a1086-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1086-113">Not supported.</span></span>|
|<span data-ttu-id="a1086-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1086-114">Application</span></span>                            |<span data-ttu-id="a1086-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1086-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="a1086-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1086-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET servicePrincipals/{id}/synchronization/templates
GET applications/{id}/synchronization/templates
```

## <a name="request-headers"></a><span data-ttu-id="a1086-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1086-117">Request headers</span></span>

| <span data-ttu-id="a1086-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a1086-118">Name</span></span>           | <span data-ttu-id="a1086-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a1086-119">Type</span></span>    | <span data-ttu-id="a1086-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a1086-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a1086-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1086-121">Authorization</span></span>  | <span data-ttu-id="a1086-122">string</span><span class="sxs-lookup"><span data-stu-id="a1086-122">string</span></span>  | <span data-ttu-id="a1086-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1086-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1086-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1086-125">Request body</span></span>

<span data-ttu-id="a1086-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1086-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="a1086-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1086-127">Response</span></span>

<span data-ttu-id="a1086-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и Аколлектион объектов [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a1086-128">If successful, this method returns a `200 OK` response code and acollection of [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) objects in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="a1086-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a1086-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a1086-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1086-130">Request</span></span>
<span data-ttu-id="a1086-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1086-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates
```

##### <a name="response"></a><span data-ttu-id="a1086-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1086-132">Response</span></span>
<span data-ttu-id="a1086-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1086-133">The following is an example of a response.</span></span>
><span data-ttu-id="a1086-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a1086-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a1086-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1086-135">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "Slack",
            "factoryTag": "CustomSCIM",
            "schema": {
                    "directories": [],
                    "synchronizationRules": []
                    }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
