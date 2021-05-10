---
title: тип ресурса unifiedRoleManagementPolicyNotificationRule
description: В единойroleManagementPolicyNotificationRule указывается правило уведомлений, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e4d8952f8ab69ed83aecde96f3bc2804affe24c8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299803"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a><span data-ttu-id="e7d80-104">тип ресурса unifiedRoleManagementPolicyNotificationRule</span><span class="sxs-lookup"><span data-stu-id="e7d80-104">unifiedRoleManagementPolicyNotificationRule resource type</span></span>

<span data-ttu-id="e7d80-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7d80-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7d80-106">В единойroleManagementPolicyNotificationRule указывается правило уведомлений, связанное с политикой управления ролью.</span><span class="sxs-lookup"><span data-stu-id="e7d80-106">A unifiedRoleManagementPolicyNotificationRule specifies the notification rule associated with a role management policy.</span></span> <span data-ttu-id="e7d80-107">Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="e7d80-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="e7d80-108">Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="e7d80-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e7d80-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7d80-109">Properties</span></span>
|<span data-ttu-id="e7d80-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7d80-110">Property</span></span>|<span data-ttu-id="e7d80-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e7d80-111">Type</span></span>|<span data-ttu-id="e7d80-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e7d80-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d80-113">id</span><span class="sxs-lookup"><span data-stu-id="e7d80-113">id</span></span>|<span data-ttu-id="e7d80-114">Строка</span><span class="sxs-lookup"><span data-stu-id="e7d80-114">String</span></span>|<span data-ttu-id="e7d80-115">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="e7d80-115">Unique identifier for the rule.</span></span> <span data-ttu-id="e7d80-116">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="e7d80-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="e7d80-117">notificationLevel</span><span class="sxs-lookup"><span data-stu-id="e7d80-117">notificationLevel</span></span>|<span data-ttu-id="e7d80-118">Строка</span><span class="sxs-lookup"><span data-stu-id="e7d80-118">String</span></span>|<span data-ttu-id="e7d80-119">Уровень уведомления.</span><span class="sxs-lookup"><span data-stu-id="e7d80-119">The level of notification.</span></span> <span data-ttu-id="e7d80-120">Один из "Нет", "Критический", "Все".</span><span class="sxs-lookup"><span data-stu-id="e7d80-120">One of None, Critical, All.</span></span>|
|<span data-ttu-id="e7d80-121">notificationRecipients</span><span class="sxs-lookup"><span data-stu-id="e7d80-121">notificationRecipients</span></span>|<span data-ttu-id="e7d80-122">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e7d80-122">String collection</span></span>|<span data-ttu-id="e7d80-123">Список уведомлений перекликается с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="e7d80-123">The list of notification recepients like email.</span></span>|
|<span data-ttu-id="e7d80-124">notificationType</span><span class="sxs-lookup"><span data-stu-id="e7d80-124">notificationType</span></span>|<span data-ttu-id="e7d80-125">Строка</span><span class="sxs-lookup"><span data-stu-id="e7d80-125">String</span></span>|<span data-ttu-id="e7d80-126">Тип уведомления.</span><span class="sxs-lookup"><span data-stu-id="e7d80-126">The type of notification.</span></span> <span data-ttu-id="e7d80-127">Одно из сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e7d80-127">One of Email.</span></span>|
|<span data-ttu-id="e7d80-128">recipientType</span><span class="sxs-lookup"><span data-stu-id="e7d80-128">recipientType</span></span>|<span data-ttu-id="e7d80-129">Строка</span><span class="sxs-lookup"><span data-stu-id="e7d80-129">String</span></span>|<span data-ttu-id="e7d80-130">Тип получателя.</span><span class="sxs-lookup"><span data-stu-id="e7d80-130">The type of recipient.</span></span> <span data-ttu-id="e7d80-131">Один из requestor, Approver, Admin.</span><span class="sxs-lookup"><span data-stu-id="e7d80-131">One of Requestor, Approver, Admin.</span></span>|
|<span data-ttu-id="e7d80-132">isDefaultRecipientsEnabled</span><span class="sxs-lookup"><span data-stu-id="e7d80-132">isDefaultRecipientsEnabled</span></span>|<span data-ttu-id="e7d80-133">Логический</span><span class="sxs-lookup"><span data-stu-id="e7d80-133">Boolean</span></span>|<span data-ttu-id="e7d80-134">Получает ли получатель электронной почты по умолчанию или нет.</span><span class="sxs-lookup"><span data-stu-id="e7d80-134">Whether default recipient is receiving the email or not.</span></span>|
|<span data-ttu-id="e7d80-135">target</span><span class="sxs-lookup"><span data-stu-id="e7d80-135">target</span></span>|[<span data-ttu-id="e7d80-136">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="e7d80-136">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="e7d80-137">Цель правила.</span><span class="sxs-lookup"><span data-stu-id="e7d80-137">The target for the rule.</span></span> <span data-ttu-id="e7d80-138">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="e7d80-138">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7d80-139">Связи</span><span class="sxs-lookup"><span data-stu-id="e7d80-139">Relationships</span></span>
<span data-ttu-id="e7d80-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e7d80-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7d80-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e7d80-141">JSON representation</span></span>
<span data-ttu-id="e7d80-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7d80-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "notificationType": "String",
  "recipientType": "String",
  "notificationLevel": "String",
  "isDefaultRecipientsEnabled": true,
  "notificationRecipients": [
    "String"
  ]
}
```

