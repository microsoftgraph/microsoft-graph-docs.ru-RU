---
title: Тип ресурса Апплиедкондитионалакцессполици
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующими действиями при входе.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e58058a174b630daa5022aed0dff78b7c2f3099
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788691"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="4e053-103">Тип ресурса Апплиедкондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="4e053-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="4e053-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e053-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e053-105">Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующими действиями при входе.</span><span class="sxs-lookup"><span data-stu-id="4e053-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="4e053-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e053-106">Properties</span></span>

| <span data-ttu-id="4e053-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e053-107">Property</span></span>   | <span data-ttu-id="4e053-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4e053-108">Type</span></span> |<span data-ttu-id="4e053-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e053-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e053-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4e053-110">displayName</span></span>|<span data-ttu-id="4e053-111">Строка</span><span class="sxs-lookup"><span data-stu-id="4e053-111">String</span></span>|<span data-ttu-id="4e053-112">Указывает имя политики условного доступа (пример: "требовать MFA для Salesforce").</span><span class="sxs-lookup"><span data-stu-id="4e053-112">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="4e053-113">енфорцедгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="4e053-113">enforcedGrantControls</span></span>|<span data-ttu-id="4e053-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4e053-114">String collection</span></span>|<span data-ttu-id="4e053-115">Указывает на элементы управления предоставлением, принудительно примененные политикой условного доступа (пример: "требовать многофакторную проверку подлинности").</span><span class="sxs-lookup"><span data-stu-id="4e053-115">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="4e053-116">енфорцедсессионконтролс</span><span class="sxs-lookup"><span data-stu-id="4e053-116">enforcedSessionControls</span></span>|<span data-ttu-id="4e053-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4e053-117">String collection</span></span>|<span data-ttu-id="4e053-118">Указывает на элементы управления сеансом, принудительно примененные политикой условного доступа (пример: "требовать принудительно заданное приложением элементов управления").</span><span class="sxs-lookup"><span data-stu-id="4e053-118">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="4e053-119">id</span><span class="sxs-lookup"><span data-stu-id="4e053-119">id</span></span>|<span data-ttu-id="4e053-120">String</span><span class="sxs-lookup"><span data-stu-id="4e053-120">String</span></span>|<span data-ttu-id="4e053-121">Уникальный идентификатор GUID политики условного доступа.</span><span class="sxs-lookup"><span data-stu-id="4e053-121">Unique GUID of the conditional access policy.</span></span>|
|<span data-ttu-id="4e053-122">result</span><span class="sxs-lookup"><span data-stu-id="4e053-122">result</span></span>|<span data-ttu-id="4e053-123">String</span><span class="sxs-lookup"><span data-stu-id="4e053-123">String</span></span>| <span data-ttu-id="4e053-124">Указывает результат политики ЦС, который был активирован.</span><span class="sxs-lookup"><span data-stu-id="4e053-124">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="4e053-125">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="4e053-125">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="4e053-126">`notApplied`-Политика не применяется, так как условия политики не выполнены.</span><span class="sxs-lookup"><span data-stu-id="4e053-126">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="4e053-127">`notEnabled`— Это связано с тем, что в отключенном состоянии политика отключена.</span><span class="sxs-lookup"><span data-stu-id="4e053-127">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e053-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e053-128">JSON representation</span></span>

<span data-ttu-id="4e053-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e053-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
