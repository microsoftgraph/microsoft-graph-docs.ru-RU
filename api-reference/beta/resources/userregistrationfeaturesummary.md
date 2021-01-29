---
title: Тип ресурса userRegistrationFeatureSummary
description: Сводка пользователей, способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 3dc3b48e6883b8c953db5d7b826243989109f2d9
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052619"
---
# <a name="userregistrationfeaturesummary-resource-type"></a><span data-ttu-id="e3f29-103">Тип ресурса userRegistrationFeatureSummary</span><span class="sxs-lookup"><span data-stu-id="e3f29-103">userRegistrationFeatureSummary resource type</span></span>

<span data-ttu-id="e3f29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3f29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3f29-105">Представляет текущее состояние того, сколько пользователей в организации могут выполнять многофакторную проверку подлинности, самостоятельный сброс паролей и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="e3f29-105">Represents the current state of how many users in your organization are capable of multi-factor authentication, self-service password reset and passwordless authentication.</span></span>

## <a name="methods"></a><span data-ttu-id="e3f29-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e3f29-106">Methods</span></span>

| <span data-ttu-id="e3f29-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e3f29-107">Method</span></span>       | <span data-ttu-id="e3f29-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e3f29-108">Return Type</span></span> | <span data-ttu-id="e3f29-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e3f29-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e3f29-110">usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="e3f29-110">usersRegisteredByFeature</span></span>](../api/authenticationmethodsroot-usersregisteredbyfeature.md) | <span data-ttu-id="e3f29-111">userRegistrationFeatureSummary</span><span class="sxs-lookup"><span data-stu-id="e3f29-111">userRegistrationFeatureSummary</span></span> | <span data-ttu-id="e3f29-112">Получите количество пользователей, способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="e3f29-112">Get the number of users capable of Multi-Factor Authentication, Self-Service Password Reset, and Passwordless authentication.</span></span> |

## <a name="properties"></a><span data-ttu-id="e3f29-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3f29-113">Properties</span></span>
|<span data-ttu-id="e3f29-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3f29-114">Property</span></span>|<span data-ttu-id="e3f29-115">Тип</span><span class="sxs-lookup"><span data-stu-id="e3f29-115">Type</span></span>|<span data-ttu-id="e3f29-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e3f29-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3f29-117">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="e3f29-117">totalUserCount</span></span>|<span data-ttu-id="e3f29-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e3f29-118">Int64</span></span>|<span data-ttu-id="e3f29-119">Общее количество учетных записей пользователей, за исключением заблокированных</span><span class="sxs-lookup"><span data-stu-id="e3f29-119">Total number of users accounts, excluding those that are blocked</span></span>|
|<span data-ttu-id="e3f29-120">userRegistrationFeatureCounts</span><span class="sxs-lookup"><span data-stu-id="e3f29-120">userRegistrationFeatureCounts</span></span>|<span data-ttu-id="e3f29-121">[Коллекция userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md)</span><span class="sxs-lookup"><span data-stu-id="e3f29-121">[userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md) collection</span></span>|<span data-ttu-id="e3f29-122">Количество пользователей, зарегистрированных или способных использовать многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="e3f29-122">Number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span>|
|<span data-ttu-id="e3f29-123">userRoles</span><span class="sxs-lookup"><span data-stu-id="e3f29-123">userRoles</span></span>|<span data-ttu-id="e3f29-124">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="e3f29-124">includedUserRoles</span></span>|<span data-ttu-id="e3f29-125">Тип роли пользователя.</span><span class="sxs-lookup"><span data-stu-id="e3f29-125">User role type.</span></span> <span data-ttu-id="e3f29-126">Возможные значения: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="e3f29-126">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|
|<span data-ttu-id="e3f29-127">userTypes</span><span class="sxs-lookup"><span data-stu-id="e3f29-127">userTypes</span></span>|<span data-ttu-id="e3f29-128">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="e3f29-128">includedUserTypes</span></span>|<span data-ttu-id="e3f29-129">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="e3f29-129">User type.</span></span> <span data-ttu-id="e3f29-130">Возможные значения: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="e3f29-130">Possible values are: `all`, `member`, `guest`.</span></span>|

<span data-ttu-id="e3f29-131">Значение состоит `privilegedAdmin` из следующих привилегированных ролей администратора:</span><span class="sxs-lookup"><span data-stu-id="e3f29-131">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="e3f29-132">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e3f29-132">Global admin</span></span>
* <span data-ttu-id="e3f29-133">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="e3f29-133">Security admin</span></span>
* <span data-ttu-id="e3f29-134">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="e3f29-134">Conditional Access admin</span></span>
* <span data-ttu-id="e3f29-135">Администратор Exchange</span><span class="sxs-lookup"><span data-stu-id="e3f29-135">Exchange admin</span></span>
* <span data-ttu-id="e3f29-136">Администратор SharePoint</span><span class="sxs-lookup"><span data-stu-id="e3f29-136">SharePoint admin</span></span>
* <span data-ttu-id="e3f29-137">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="e3f29-137">Helpdesk admin</span></span>
* <span data-ttu-id="e3f29-138">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="e3f29-138">Billing admin</span></span>
* <span data-ttu-id="e3f29-139">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="e3f29-139">User admin</span></span>
* <span data-ttu-id="e3f29-140">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="e3f29-140">Authentication admin</span></span>

<span data-ttu-id="e3f29-141">Значение включает `admin` все роли администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e3f29-141">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="relationships"></a><span data-ttu-id="e3f29-142">Связи</span><span class="sxs-lookup"><span data-stu-id="e3f29-142">Relationships</span></span>
<span data-ttu-id="e3f29-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e3f29-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3f29-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3f29-144">JSON representation</span></span>
<span data-ttu-id="e3f29-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3f29-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationFeatureCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
    }
  ]
}
```
