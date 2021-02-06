---
title: Тип ресурса userRegistrationFeatureSummary
description: Сводка пользователей, способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 291da483380d6e1d65b5db527128098b8b416c83
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132937"
---
# <a name="userregistrationfeaturesummary-resource-type"></a><span data-ttu-id="78c0d-103">Тип ресурса userRegistrationFeatureSummary</span><span class="sxs-lookup"><span data-stu-id="78c0d-103">userRegistrationFeatureSummary resource type</span></span>

<span data-ttu-id="78c0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78c0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78c0d-105">Представляет текущее состояние того, сколько пользователей в организации могут выполнять многофакторную проверку подлинности, самостоятельный сброс паролей и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="78c0d-105">Represents the current state of how many users in your organization are capable of multi-factor authentication, self-service password reset and passwordless authentication.</span></span>

## <a name="methods"></a><span data-ttu-id="78c0d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="78c0d-106">Methods</span></span>

| <span data-ttu-id="78c0d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="78c0d-107">Method</span></span>       | <span data-ttu-id="78c0d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="78c0d-108">Return Type</span></span> | <span data-ttu-id="78c0d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="78c0d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="78c0d-110">usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="78c0d-110">usersRegisteredByFeature</span></span>](../api/authenticationmethodsroot-usersregisteredbyfeature.md) | <span data-ttu-id="78c0d-111">userRegistrationFeatureSummary</span><span class="sxs-lookup"><span data-stu-id="78c0d-111">userRegistrationFeatureSummary</span></span> | <span data-ttu-id="78c0d-112">Получите количество пользователей, способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="78c0d-112">Get the number of users capable of Multi-Factor Authentication, Self-Service Password Reset, and Passwordless authentication.</span></span> |

## <a name="properties"></a><span data-ttu-id="78c0d-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="78c0d-113">Properties</span></span>
|<span data-ttu-id="78c0d-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="78c0d-114">Property</span></span>|<span data-ttu-id="78c0d-115">Тип</span><span class="sxs-lookup"><span data-stu-id="78c0d-115">Type</span></span>|<span data-ttu-id="78c0d-116">Описание</span><span class="sxs-lookup"><span data-stu-id="78c0d-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78c0d-117">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="78c0d-117">totalUserCount</span></span>|<span data-ttu-id="78c0d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="78c0d-118">Int64</span></span>|<span data-ttu-id="78c0d-119">Общее количество учетных записей пользователей, за исключением заблокированных</span><span class="sxs-lookup"><span data-stu-id="78c0d-119">Total number of users accounts, excluding those that are blocked</span></span>|
|<span data-ttu-id="78c0d-120">userRegistrationFeatureCounts</span><span class="sxs-lookup"><span data-stu-id="78c0d-120">userRegistrationFeatureCounts</span></span>|<span data-ttu-id="78c0d-121">[Коллекция userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md)</span><span class="sxs-lookup"><span data-stu-id="78c0d-121">[userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md) collection</span></span>|<span data-ttu-id="78c0d-122">Количество пользователей, зарегистрированных или способных использовать многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="78c0d-122">Number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span>|
|<span data-ttu-id="78c0d-123">userRoles</span><span class="sxs-lookup"><span data-stu-id="78c0d-123">userRoles</span></span>|<span data-ttu-id="78c0d-124">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="78c0d-124">includedUserRoles</span></span>|<span data-ttu-id="78c0d-125">Тип роли пользователя.</span><span class="sxs-lookup"><span data-stu-id="78c0d-125">User role type.</span></span> <span data-ttu-id="78c0d-126">Возможные значения: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="78c0d-126">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|
|<span data-ttu-id="78c0d-127">userTypes</span><span class="sxs-lookup"><span data-stu-id="78c0d-127">userTypes</span></span>|<span data-ttu-id="78c0d-128">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="78c0d-128">includedUserTypes</span></span>|<span data-ttu-id="78c0d-129">Тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="78c0d-129">User type.</span></span> <span data-ttu-id="78c0d-130">Возможные значения: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="78c0d-130">Possible values are: `all`, `member`, `guest`.</span></span>|

<span data-ttu-id="78c0d-131">Значение состоит `privilegedAdmin` из следующих привилегированных ролей администратора:</span><span class="sxs-lookup"><span data-stu-id="78c0d-131">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="78c0d-132">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="78c0d-132">Global admin</span></span>
* <span data-ttu-id="78c0d-133">Администратор безопасности</span><span class="sxs-lookup"><span data-stu-id="78c0d-133">Security admin</span></span>
* <span data-ttu-id="78c0d-134">Администратор условного доступа</span><span class="sxs-lookup"><span data-stu-id="78c0d-134">Conditional Access admin</span></span>
* <span data-ttu-id="78c0d-135">Администратор Exchange</span><span class="sxs-lookup"><span data-stu-id="78c0d-135">Exchange admin</span></span>
* <span data-ttu-id="78c0d-136">Администратор SharePoint</span><span class="sxs-lookup"><span data-stu-id="78c0d-136">SharePoint admin</span></span>
* <span data-ttu-id="78c0d-137">Администратор службы поддержки</span><span class="sxs-lookup"><span data-stu-id="78c0d-137">Helpdesk admin</span></span>
* <span data-ttu-id="78c0d-138">Администратор выставления счетов</span><span class="sxs-lookup"><span data-stu-id="78c0d-138">Billing admin</span></span>
* <span data-ttu-id="78c0d-139">Администратор пользователей</span><span class="sxs-lookup"><span data-stu-id="78c0d-139">User admin</span></span>
* <span data-ttu-id="78c0d-140">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="78c0d-140">Authentication admin</span></span>

<span data-ttu-id="78c0d-141">Это значение `admin` включает все роли администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="78c0d-141">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="relationships"></a><span data-ttu-id="78c0d-142">Связи</span><span class="sxs-lookup"><span data-stu-id="78c0d-142">Relationships</span></span>
<span data-ttu-id="78c0d-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="78c0d-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78c0d-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="78c0d-144">JSON representation</span></span>
<span data-ttu-id="78c0d-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78c0d-145">The following is a JSON representation of the resource.</span></span>
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
