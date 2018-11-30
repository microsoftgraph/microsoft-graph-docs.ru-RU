---
title: Создание groupLifecyclePolicy
description: Создает объект groupLifecyclePolicy.
ms.openlocfilehash: ee7b4665f68bbbfeae268d7f86c10fa433c46cd3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082088"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="9c57c-103">Создание groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9c57c-103">Create groupLifecyclePolicy</span></span>

> <span data-ttu-id="9c57c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c57c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c57c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c57c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c57c-106">Создает объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9c57c-106">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c57c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c57c-107">Permissions</span></span>

<span data-ttu-id="9c57c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c57c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9c57c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c57c-110">Permission type</span></span>      | <span data-ttu-id="9c57c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c57c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c57c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c57c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c57c-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c57c-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c57c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c57c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c57c-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9c57c-115">Not supported</span></span> |
|<span data-ttu-id="9c57c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c57c-116">Application</span></span> |  <span data-ttu-id="9c57c-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c57c-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c57c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c57c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="9c57c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c57c-119">Request headers</span></span>

| <span data-ttu-id="9c57c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9c57c-120">Name</span></span> | <span data-ttu-id="9c57c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9c57c-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9c57c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c57c-122">Authorization</span></span> | <span data-ttu-id="9c57c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c57c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c57c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c57c-125">Content-Type</span></span>  | <span data-ttu-id="9c57c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c57c-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c57c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c57c-127">Request body</span></span>
<span data-ttu-id="9c57c-128">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c57c-128">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9c57c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c57c-129">Response</span></span>

<span data-ttu-id="9c57c-130">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9c57c-130">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c57c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9c57c-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9c57c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c57c-132">Request</span></span>

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
<span data-ttu-id="9c57c-133">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c57c-133">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9c57c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c57c-134">Response</span></span>

<span data-ttu-id="9c57c-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c57c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->