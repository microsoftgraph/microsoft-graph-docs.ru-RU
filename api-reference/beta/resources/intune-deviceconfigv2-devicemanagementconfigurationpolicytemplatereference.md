---
title: тип ресурса deviceManagementConfigurationPolicyTemplateReference
description: Справочные сведения шаблона политики
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dee3cf25ed42f2c1ecdbf824fd807ed00c8ce91b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868911"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a><span data-ttu-id="d7db4-103">тип ресурса deviceManagementConfigurationPolicyTemplateReference</span><span class="sxs-lookup"><span data-stu-id="d7db4-103">deviceManagementConfigurationPolicyTemplateReference resource type</span></span>

<span data-ttu-id="d7db4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7db4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7db4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7db4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7db4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7db4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7db4-107">Справочные сведения шаблона политики</span><span class="sxs-lookup"><span data-stu-id="d7db4-107">Policy template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="d7db4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7db4-108">Properties</span></span>
|<span data-ttu-id="d7db4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7db4-109">Property</span></span>|<span data-ttu-id="d7db4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7db4-110">Type</span></span>|<span data-ttu-id="d7db4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7db4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7db4-112">templateId</span><span class="sxs-lookup"><span data-stu-id="d7db4-112">templateId</span></span>|<span data-ttu-id="d7db4-113">String</span><span class="sxs-lookup"><span data-stu-id="d7db4-113">String</span></span>|<span data-ttu-id="d7db4-114">Шаблон id</span><span class="sxs-lookup"><span data-stu-id="d7db4-114">Template id</span></span>|
|<span data-ttu-id="d7db4-115">templateFamily</span><span class="sxs-lookup"><span data-stu-id="d7db4-115">templateFamily</span></span>|[<span data-ttu-id="d7db4-116">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="d7db4-116">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="d7db4-117">Семейство шаблонов ссылаемого шаблона.</span><span class="sxs-lookup"><span data-stu-id="d7db4-117">Template Family of the referenced Template.</span></span> <span data-ttu-id="d7db4-118">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7db4-118">This property is read-only.</span></span> <span data-ttu-id="d7db4-119">Возможные значения: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span><span class="sxs-lookup"><span data-stu-id="d7db4-119">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="d7db4-120">templateDisplayName</span><span class="sxs-lookup"><span data-stu-id="d7db4-120">templateDisplayName</span></span>|<span data-ttu-id="d7db4-121">String</span><span class="sxs-lookup"><span data-stu-id="d7db4-121">String</span></span>|<span data-ttu-id="d7db4-122">Отображение имени шаблона ссылаемого шаблона.</span><span class="sxs-lookup"><span data-stu-id="d7db4-122">Template Display Name of the referenced template.</span></span> <span data-ttu-id="d7db4-123">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7db4-123">This property is read-only.</span></span>|
|<span data-ttu-id="d7db4-124">templateDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="d7db4-124">templateDisplayVersion</span></span>|<span data-ttu-id="d7db4-125">String</span><span class="sxs-lookup"><span data-stu-id="d7db4-125">String</span></span>|<span data-ttu-id="d7db4-126">Отображение шаблона версии ссылаемого шаблона.</span><span class="sxs-lookup"><span data-stu-id="d7db4-126">Template Display Version of the referenced Template.</span></span> <span data-ttu-id="d7db4-127">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7db4-127">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7db4-128">Связи</span><span class="sxs-lookup"><span data-stu-id="d7db4-128">Relationships</span></span>
<span data-ttu-id="d7db4-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d7db4-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7db4-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7db4-130">JSON Representation</span></span>
<span data-ttu-id="d7db4-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7db4-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
  "templateId": "String",
  "templateFamily": "String",
  "templateDisplayName": "String",
  "templateDisplayVersion": "String"
}
```




