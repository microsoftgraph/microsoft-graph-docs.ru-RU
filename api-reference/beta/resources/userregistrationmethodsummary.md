---
title: Тип ресурса userRegistrationMethodSummary
description: Сводка количества пользователей, зарегистрированных для каждого метода проверки подлинности.
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6ff9a079ddce0df5031eef2b1374ebb1d233d56d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132925"
---
# <a name="userregistrationmethodsummary-resource-type"></a><span data-ttu-id="983fa-103">Тип ресурса userRegistrationMethodSummary</span><span class="sxs-lookup"><span data-stu-id="983fa-103">userRegistrationMethodSummary resource type</span></span>

<span data-ttu-id="983fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="983fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="983fa-105">Сводка количества пользователей, зарегистрированных для каждого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="983fa-105">Summary of number of users registered for each authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="983fa-106">Методы</span><span class="sxs-lookup"><span data-stu-id="983fa-106">Methods</span></span>

| <span data-ttu-id="983fa-107">Метод</span><span class="sxs-lookup"><span data-stu-id="983fa-107">Method</span></span>       | <span data-ttu-id="983fa-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="983fa-108">Return Type</span></span> | <span data-ttu-id="983fa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="983fa-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="983fa-110">usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="983fa-110">usersRegisteredByMethod</span></span>](../api/authenticationmethodsroot-usersregisteredbymethod.md) | <span data-ttu-id="983fa-111">userRegistrationMethodSummary</span><span class="sxs-lookup"><span data-stu-id="983fa-111">userRegistrationMethodSummary</span></span> | <span data-ttu-id="983fa-112">Получите количество пользователей, зарегистрированных для каждого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="983fa-112">Get the number of users registered for each authentication method.</span></span> |

## <a name="properties"></a><span data-ttu-id="983fa-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="983fa-113">Properties</span></span>
|<span data-ttu-id="983fa-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="983fa-114">Property</span></span>|<span data-ttu-id="983fa-115">Тип</span><span class="sxs-lookup"><span data-stu-id="983fa-115">Type</span></span>|<span data-ttu-id="983fa-116">Описание</span><span class="sxs-lookup"><span data-stu-id="983fa-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="983fa-117">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="983fa-117">totalUserCount</span></span>|<span data-ttu-id="983fa-118">Int64</span><span class="sxs-lookup"><span data-stu-id="983fa-118">Int64</span></span>|<span data-ttu-id="983fa-119">Общее количество пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="983fa-119">Total number of users in the tenant.</span></span>|
|<span data-ttu-id="983fa-120">userRegistrationMethodCounts</span><span class="sxs-lookup"><span data-stu-id="983fa-120">userRegistrationMethodCounts</span></span>|<span data-ttu-id="983fa-121">[Коллекция userRegistrationMethodCount](../resources/userregistrationmethodcount.md)</span><span class="sxs-lookup"><span data-stu-id="983fa-121">[userRegistrationMethodCount](../resources/userregistrationmethodcount.md) collection</span></span>|<span data-ttu-id="983fa-122">Количество пользователей, зарегистрированных для каждого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="983fa-122">Number of users registered for each authentication method.</span></span>|
|<span data-ttu-id="983fa-123">userRoles</span><span class="sxs-lookup"><span data-stu-id="983fa-123">userRoles</span></span>|<span data-ttu-id="983fa-124">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="983fa-124">includedUserRoles</span></span>|<span data-ttu-id="983fa-125">Тип роли пользователя.</span><span class="sxs-lookup"><span data-stu-id="983fa-125">User role type.</span></span> <span data-ttu-id="983fa-126">Возможные значения: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="983fa-126">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|
|<span data-ttu-id="983fa-127">userTypes</span><span class="sxs-lookup"><span data-stu-id="983fa-127">userTypes</span></span>|<span data-ttu-id="983fa-128">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="983fa-128">includedUserTypes</span></span>|<span data-ttu-id="983fa-129">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="983fa-129">User type.</span></span> <span data-ttu-id="983fa-130">Возможные значения: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="983fa-130">Possible values are: `all`, `member`, `guest`.</span></span>|

<span data-ttu-id="983fa-131">Значение состоит `privilegedAdmin` из следующих привилегированных ролей администратора:</span><span class="sxs-lookup"><span data-stu-id="983fa-131">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="983fa-132">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="983fa-132">Global admin</span></span>
* <span data-ttu-id="983fa-133">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="983fa-133">Security admin</span></span>
* <span data-ttu-id="983fa-134">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="983fa-134">Conditional Access admin</span></span>
* <span data-ttu-id="983fa-135">Администратор Exchange</span><span class="sxs-lookup"><span data-stu-id="983fa-135">Exchange admin</span></span>
* <span data-ttu-id="983fa-136">Администратор SharePoint</span><span class="sxs-lookup"><span data-stu-id="983fa-136">SharePoint admin</span></span>
* <span data-ttu-id="983fa-137">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="983fa-137">Helpdesk admin</span></span>
* <span data-ttu-id="983fa-138">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="983fa-138">Billing admin</span></span>
* <span data-ttu-id="983fa-139">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="983fa-139">User admin</span></span>
* <span data-ttu-id="983fa-140">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="983fa-140">Authentication admin</span></span>

<span data-ttu-id="983fa-141">Значение включает `admin` все роли администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="983fa-141">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="relationships"></a><span data-ttu-id="983fa-142">Связи</span><span class="sxs-lookup"><span data-stu-id="983fa-142">Relationships</span></span>
<span data-ttu-id="983fa-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="983fa-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="983fa-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="983fa-144">JSON representation</span></span>
<span data-ttu-id="983fa-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="983fa-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationMethodCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationMethodCount"
    }
  ]
}
```
