---
title: тип ресурса deviceManagementConfigurationReferenceSettingValue
description: Модель для ReferenceSettingValue
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1dc92606270cf4c2febcee68905f0c8bd29ced13
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868908"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a><span data-ttu-id="0376f-103">тип ресурса deviceManagementConfigurationReferenceSettingValue</span><span class="sxs-lookup"><span data-stu-id="0376f-103">deviceManagementConfigurationReferenceSettingValue resource type</span></span>

<span data-ttu-id="0376f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0376f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0376f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0376f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0376f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0376f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0376f-107">Модель для ReferenceSettingValue</span><span class="sxs-lookup"><span data-stu-id="0376f-107">Model for ReferenceSettingValue</span></span>


<span data-ttu-id="0376f-108">Наследует [от deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0376f-108">Inherits from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0376f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0376f-109">Properties</span></span>
|<span data-ttu-id="0376f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0376f-110">Property</span></span>|<span data-ttu-id="0376f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0376f-111">Type</span></span>|<span data-ttu-id="0376f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0376f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0376f-113">значение</span><span class="sxs-lookup"><span data-stu-id="0376f-113">value</span></span>|<span data-ttu-id="0376f-114">String</span><span class="sxs-lookup"><span data-stu-id="0376f-114">String</span></span>|<span data-ttu-id="0376f-115">Значение параметра строки.</span><span class="sxs-lookup"><span data-stu-id="0376f-115">Value of the string setting.</span></span> <span data-ttu-id="0376f-116">Унаследованный от [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0376f-116">Inherited from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>|
|<span data-ttu-id="0376f-117">примечание</span><span class="sxs-lookup"><span data-stu-id="0376f-117">note</span></span>|<span data-ttu-id="0376f-118">String</span><span class="sxs-lookup"><span data-stu-id="0376f-118">String</span></span>|<span data-ttu-id="0376f-119">Примечание, которое администратор может использовать для вложения определенных контекстных сведений</span><span class="sxs-lookup"><span data-stu-id="0376f-119">A note that admin can use to put some contextual information</span></span>|

## <a name="relationships"></a><span data-ttu-id="0376f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="0376f-120">Relationships</span></span>
<span data-ttu-id="0376f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0376f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0376f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0376f-122">JSON Representation</span></span>
<span data-ttu-id="0376f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0376f-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferenceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferenceSettingValue",
  "value": "String",
  "note": "String"
}
```




