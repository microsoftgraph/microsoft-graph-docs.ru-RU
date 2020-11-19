---
title: Тип ресурса Секуритибаселинеконтрибутингполици
description: Состояние соответствия базовой безопасности параметру для устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f62299f39d4e3670fc586a4dc07d352a992398e0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209348"
---
# <a name="securitybaselinecontributingpolicy-resource-type"></a><span data-ttu-id="77fc4-103">Тип ресурса Секуритибаселинеконтрибутингполици</span><span class="sxs-lookup"><span data-stu-id="77fc4-103">securityBaselineContributingPolicy resource type</span></span>

<span data-ttu-id="77fc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77fc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77fc4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77fc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77fc4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77fc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77fc4-107">Состояние соответствия базовой безопасности параметру для устройства</span><span class="sxs-lookup"><span data-stu-id="77fc4-107">The security baseline compliance state of a setting for a device</span></span>

## <a name="properties"></a><span data-ttu-id="77fc4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="77fc4-108">Properties</span></span>
|<span data-ttu-id="77fc4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="77fc4-109">Property</span></span>|<span data-ttu-id="77fc4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="77fc4-110">Type</span></span>|<span data-ttu-id="77fc4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="77fc4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77fc4-112">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="77fc4-112">sourceId</span></span>|<span data-ttu-id="77fc4-113">String</span><span class="sxs-lookup"><span data-stu-id="77fc4-113">String</span></span>|<span data-ttu-id="77fc4-114">Уникальный идентификатор политики</span><span class="sxs-lookup"><span data-stu-id="77fc4-114">Unique identifier of the policy</span></span>|
|<span data-ttu-id="77fc4-115">displayName</span><span class="sxs-lookup"><span data-stu-id="77fc4-115">displayName</span></span>|<span data-ttu-id="77fc4-116">String</span><span class="sxs-lookup"><span data-stu-id="77fc4-116">String</span></span>|<span data-ttu-id="77fc4-117">Имя политики</span><span class="sxs-lookup"><span data-stu-id="77fc4-117">Name of the policy</span></span>|
|<span data-ttu-id="77fc4-118">sourceType</span><span class="sxs-lookup"><span data-stu-id="77fc4-118">sourceType</span></span>|[<span data-ttu-id="77fc4-119">секуритибаселинеполицисаурцетипе</span><span class="sxs-lookup"><span data-stu-id="77fc4-119">securityBaselinePolicySourceType</span></span>](../resources/intune-deviceintent-securitybaselinepolicysourcetype.md)|<span data-ttu-id="77fc4-120">Источник создания политики.</span><span class="sxs-lookup"><span data-stu-id="77fc4-120">Authoring source of the policy.</span></span> <span data-ttu-id="77fc4-121">Возможные значения: `deviceConfiguration`, `deviceIntent`.</span><span class="sxs-lookup"><span data-stu-id="77fc4-121">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77fc4-122">Связи</span><span class="sxs-lookup"><span data-stu-id="77fc4-122">Relationships</span></span>
<span data-ttu-id="77fc4-123">Нет</span><span class="sxs-lookup"><span data-stu-id="77fc4-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77fc4-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77fc4-124">JSON Representation</span></span>
<span data-ttu-id="77fc4-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77fc4-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.securityBaselineContributingPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineContributingPolicy",
  "sourceId": "String",
  "displayName": "String",
  "sourceType": "String"
}
```




