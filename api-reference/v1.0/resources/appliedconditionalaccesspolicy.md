---
title: Тип ресурса Апплиедкондитионалакцессполици
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующими действиями при входе.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d8b569436152e2a57e152f0fe2f2c632f0d2d93a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033252"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="040dc-103">Тип ресурса Апплиедкондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="040dc-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="040dc-104">Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующими действиями при входе.</span><span class="sxs-lookup"><span data-stu-id="040dc-104">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="040dc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="040dc-105">Properties</span></span>

| <span data-ttu-id="040dc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="040dc-106">Property</span></span>   | <span data-ttu-id="040dc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="040dc-107">Type</span></span> |<span data-ttu-id="040dc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="040dc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="040dc-109">displayName</span><span class="sxs-lookup"><span data-stu-id="040dc-109">displayName</span></span>|<span data-ttu-id="040dc-110">Строка</span><span class="sxs-lookup"><span data-stu-id="040dc-110">String</span></span>|<span data-ttu-id="040dc-111">Указывает имя политики условного доступа (пример: "требовать MFA для Salesforce").</span><span class="sxs-lookup"><span data-stu-id="040dc-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="040dc-112">Енфорцедгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="040dc-112">enforcedGrantControls</span></span>|<span data-ttu-id="040dc-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="040dc-113">String collection</span></span>|<span data-ttu-id="040dc-114">Указывает на элементы управления предоставлением, принудительно примененные политикой условного доступа (пример: "требовать многофакторную проверку подлинности").</span><span class="sxs-lookup"><span data-stu-id="040dc-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="040dc-115">Енфорцедсессионконтролс</span><span class="sxs-lookup"><span data-stu-id="040dc-115">enforcedSessionControls</span></span>|<span data-ttu-id="040dc-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="040dc-116">String collection</span></span>|<span data-ttu-id="040dc-117">Указывает на элементы управления сеансом, принудительно примененные политикой условного доступа (пример: "требовать принудительно заданное приложением элементов управления").</span><span class="sxs-lookup"><span data-stu-id="040dc-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="040dc-118">id</span><span class="sxs-lookup"><span data-stu-id="040dc-118">id</span></span>|<span data-ttu-id="040dc-119">String</span><span class="sxs-lookup"><span data-stu-id="040dc-119">String</span></span>|<span data-ttu-id="040dc-120">Уникальный идентификатор GUID для условного доступа полик. y</span><span class="sxs-lookup"><span data-stu-id="040dc-120">Unique GUID of the conditional access polic.y</span></span>|
|<span data-ttu-id="040dc-121">result</span><span class="sxs-lookup"><span data-stu-id="040dc-121">result</span></span>|<span data-ttu-id="040dc-122">String</span><span class="sxs-lookup"><span data-stu-id="040dc-122">String</span></span>| <span data-ttu-id="040dc-123">Указывает результат политики ЦС, который был активирован.</span><span class="sxs-lookup"><span data-stu-id="040dc-123">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="040dc-124">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="040dc-124">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="040dc-125">`notApplied`-Политика не применяется, так как условия политики не выполнены.</span><span class="sxs-lookup"><span data-stu-id="040dc-125">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="040dc-126">`notEnabled`— Это связано с тем, что в отключенном состоянии политика отключена.</span><span class="sxs-lookup"><span data-stu-id="040dc-126">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="040dc-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="040dc-127">JSON representation</span></span>

<span data-ttu-id="040dc-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="040dc-128">Here is a JSON representation of the resource.</span></span>

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
