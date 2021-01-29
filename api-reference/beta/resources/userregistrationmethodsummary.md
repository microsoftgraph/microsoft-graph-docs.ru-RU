---
title: Тип ресурса userRegistrationMethodSummary
description: Сводка количества пользователей, зарегистрированных для каждого метода проверки подлинности.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 4f4d391291008bcbca1d017360bcb8caf3aea067
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052622"
---
# <a name="userregistrationmethodsummary-resource-type"></a><span data-ttu-id="e4a6e-103">Тип ресурса userRegistrationMethodSummary</span><span class="sxs-lookup"><span data-stu-id="e4a6e-103">userRegistrationMethodSummary resource type</span></span>

<span data-ttu-id="e4a6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4a6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4a6e-105">Сводка количества пользователей, зарегистрированных для каждого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-105">Summary of number of users registered for each authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="e4a6e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e4a6e-106">Methods</span></span>

| <span data-ttu-id="e4a6e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e4a6e-107">Method</span></span>       | <span data-ttu-id="e4a6e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e4a6e-108">Return Type</span></span> | <span data-ttu-id="e4a6e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4a6e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e4a6e-110">usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="e4a6e-110">usersRegisteredByMethod</span></span>](../api/authenticationmethodsroot-usersregisteredbymethod.md) | <span data-ttu-id="e4a6e-111">userRegistrationMethodSummary</span><span class="sxs-lookup"><span data-stu-id="e4a6e-111">userRegistrationMethodSummary</span></span> | <span data-ttu-id="e4a6e-112">Получите количество пользователей, зарегистрированных для каждого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-112">Get the number of users registered for each authentication method.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4a6e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4a6e-113">Properties</span></span>
|<span data-ttu-id="e4a6e-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4a6e-114">Property</span></span>|<span data-ttu-id="e4a6e-115">Тип</span><span class="sxs-lookup"><span data-stu-id="e4a6e-115">Type</span></span>|<span data-ttu-id="e4a6e-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e4a6e-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4a6e-117">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="e4a6e-117">totalUserCount</span></span>|<span data-ttu-id="e4a6e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e4a6e-118">Int64</span></span>|<span data-ttu-id="e4a6e-119">Общее количество пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-119">Total number of users in the tenant.</span></span>|
|<span data-ttu-id="e4a6e-120">userRegistrationMethodCounts</span><span class="sxs-lookup"><span data-stu-id="e4a6e-120">userRegistrationMethodCounts</span></span>|<span data-ttu-id="e4a6e-121">[Коллекция userRegistrationMethodCount](../resources/userregistrationmethodcount.md)</span><span class="sxs-lookup"><span data-stu-id="e4a6e-121">[userRegistrationMethodCount](../resources/userregistrationmethodcount.md) collection</span></span>|<span data-ttu-id="e4a6e-122">Количество пользователей, зарегистрированных для каждого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-122">Number of users registered for each authentication method.</span></span>|
|<span data-ttu-id="e4a6e-123">userRoles</span><span class="sxs-lookup"><span data-stu-id="e4a6e-123">userRoles</span></span>|<span data-ttu-id="e4a6e-124">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="e4a6e-124">includedUserRoles</span></span>|<span data-ttu-id="e4a6e-125">Тип роли пользователя.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-125">User role type.</span></span> <span data-ttu-id="e4a6e-126">Возможные значения: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-126">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|
|<span data-ttu-id="e4a6e-127">userTypes</span><span class="sxs-lookup"><span data-stu-id="e4a6e-127">userTypes</span></span>|<span data-ttu-id="e4a6e-128">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="e4a6e-128">includedUserTypes</span></span>|<span data-ttu-id="e4a6e-129">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-129">User type.</span></span> <span data-ttu-id="e4a6e-130">Возможные значения: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-130">Possible values are: `all`, `member`, `guest`.</span></span>|

<span data-ttu-id="e4a6e-131">Значение состоит `privilegedAdmin` из следующих привилегированных ролей администратора:</span><span class="sxs-lookup"><span data-stu-id="e4a6e-131">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="e4a6e-132">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e4a6e-132">Global admin</span></span>
* <span data-ttu-id="e4a6e-133">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="e4a6e-133">Security admin</span></span>
* <span data-ttu-id="e4a6e-134">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="e4a6e-134">Conditional Access admin</span></span>
* <span data-ttu-id="e4a6e-135">Администратор Exchange</span><span class="sxs-lookup"><span data-stu-id="e4a6e-135">Exchange admin</span></span>
* <span data-ttu-id="e4a6e-136">Администратор SharePoint</span><span class="sxs-lookup"><span data-stu-id="e4a6e-136">SharePoint admin</span></span>
* <span data-ttu-id="e4a6e-137">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="e4a6e-137">Helpdesk admin</span></span>
* <span data-ttu-id="e4a6e-138">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="e4a6e-138">Billing admin</span></span>
* <span data-ttu-id="e4a6e-139">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="e4a6e-139">User admin</span></span>
* <span data-ttu-id="e4a6e-140">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e4a6e-140">Authentication admin</span></span>

<span data-ttu-id="e4a6e-141">Значение включает `admin` все роли администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-141">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="relationships"></a><span data-ttu-id="e4a6e-142">Связи</span><span class="sxs-lookup"><span data-stu-id="e4a6e-142">Relationships</span></span>
<span data-ttu-id="e4a6e-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4a6e-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e4a6e-144">JSON representation</span></span>
<span data-ttu-id="e4a6e-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4a6e-145">The following is a JSON representation of the resource.</span></span>
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