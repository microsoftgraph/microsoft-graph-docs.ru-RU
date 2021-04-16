---
title: тип ресурса deviceManagementConfigurationReferredSettingInformation
description: Переданные сведения о параметре повторного параметров
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12003df5ec19bdf32b213945033eb9d5e73b9692
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868806"
---
# <a name="devicemanagementconfigurationreferredsettinginformation-resource-type"></a><span data-ttu-id="cfe4b-103">тип ресурса deviceManagementConfigurationReferredSettingInformation</span><span class="sxs-lookup"><span data-stu-id="cfe4b-103">deviceManagementConfigurationReferredSettingInformation resource type</span></span>

<span data-ttu-id="cfe4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfe4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfe4b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfe4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfe4b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cfe4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfe4b-107">Переданные сведения о параметре повторного параметров</span><span class="sxs-lookup"><span data-stu-id="cfe4b-107">Referred setting information about reusable setting</span></span>

## <a name="properties"></a><span data-ttu-id="cfe4b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfe4b-108">Properties</span></span>
|<span data-ttu-id="cfe4b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfe4b-109">Property</span></span>|<span data-ttu-id="cfe4b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cfe4b-110">Type</span></span>|<span data-ttu-id="cfe4b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cfe4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe4b-112">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cfe4b-112">settingDefinitionId</span></span>|<span data-ttu-id="cfe4b-113">String</span><span class="sxs-lookup"><span data-stu-id="cfe4b-113">String</span></span>|<span data-ttu-id="cfe4b-114">Настройка id определения, который ссылается на параметр.</span><span class="sxs-lookup"><span data-stu-id="cfe4b-114">Setting definition id that is being referred to a setting.</span></span> <span data-ttu-id="cfe4b-115">Применимо для повторного параметров</span><span class="sxs-lookup"><span data-stu-id="cfe4b-115">Applicable for reusable setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfe4b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="cfe4b-116">Relationships</span></span>
<span data-ttu-id="cfe4b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="cfe4b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfe4b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfe4b-118">JSON Representation</span></span>
<span data-ttu-id="cfe4b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfe4b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
  "settingDefinitionId": "String"
}
```




