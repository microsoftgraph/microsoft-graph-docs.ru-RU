---
title: Создание groupLifecyclePolicy
description: Создает объект groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 311b2b5e499bcfea0622f457d76c7a60aaef2741
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328498"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="7e7b5-103">Создание groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7e7b5-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e7b5-104">Создает объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7e7b5-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e7b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e7b5-105">Permissions</span></span>

<span data-ttu-id="7e7b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e7b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7e7b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e7b5-108">Permission type</span></span>      | <span data-ttu-id="7e7b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e7b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e7b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e7b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e7b5-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e7b5-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e7b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e7b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e7b5-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7e7b5-113">Not supported</span></span> |
|<span data-ttu-id="7e7b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e7b5-114">Application</span></span> |  <span data-ttu-id="7e7b5-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e7b5-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e7b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e7b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="7e7b5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e7b5-117">Request headers</span></span>

| <span data-ttu-id="7e7b5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7e7b5-118">Name</span></span> | <span data-ttu-id="7e7b5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7e7b5-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7e7b5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e7b5-120">Authorization</span></span> | <span data-ttu-id="7e7b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e7b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e7b5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e7b5-123">Content-Type</span></span>  | <span data-ttu-id="7e7b5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7e7b5-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e7b5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e7b5-125">Request body</span></span>
<span data-ttu-id="7e7b5-126">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e7b5-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7e7b5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e7b5-127">Response</span></span>

<span data-ttu-id="7e7b5-128">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e7b5-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e7b5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7e7b5-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e7b5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e7b5-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="7e7b5-131">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e7b5-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7e7b5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e7b5-132">Response</span></span>

<span data-ttu-id="7e7b5-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e7b5-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
