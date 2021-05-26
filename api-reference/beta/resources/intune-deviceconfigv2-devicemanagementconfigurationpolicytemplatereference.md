---
title: тип ресурса deviceManagementConfigurationPolicyTemplateReference
description: Справочные сведения шаблона политики
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff61ac1e881ec6bb40750d9cb43d80c6722dd79e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666501"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a><span data-ttu-id="c199f-103">тип ресурса deviceManagementConfigurationPolicyTemplateReference</span><span class="sxs-lookup"><span data-stu-id="c199f-103">deviceManagementConfigurationPolicyTemplateReference resource type</span></span>

<span data-ttu-id="c199f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c199f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c199f-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c199f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c199f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c199f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c199f-107">Справочные сведения шаблона политики</span><span class="sxs-lookup"><span data-stu-id="c199f-107">Policy template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="c199f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c199f-108">Properties</span></span>
|<span data-ttu-id="c199f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c199f-109">Property</span></span>|<span data-ttu-id="c199f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c199f-110">Type</span></span>|<span data-ttu-id="c199f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c199f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c199f-112">templateId</span><span class="sxs-lookup"><span data-stu-id="c199f-112">templateId</span></span>|<span data-ttu-id="c199f-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c199f-113">String</span></span>|<span data-ttu-id="c199f-114">Шаблон id</span><span class="sxs-lookup"><span data-stu-id="c199f-114">Template id</span></span>|
|<span data-ttu-id="c199f-115">templateFamily</span><span class="sxs-lookup"><span data-stu-id="c199f-115">templateFamily</span></span>|[<span data-ttu-id="c199f-116">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="c199f-116">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="c199f-117">Семейство шаблонов ссылаемого шаблона.</span><span class="sxs-lookup"><span data-stu-id="c199f-117">Template Family of the referenced Template.</span></span> <span data-ttu-id="c199f-118">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c199f-118">This property is read-only.</span></span> <span data-ttu-id="c199f-119">Возможные значения: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span><span class="sxs-lookup"><span data-stu-id="c199f-119">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="c199f-120">templateDisplayName</span><span class="sxs-lookup"><span data-stu-id="c199f-120">templateDisplayName</span></span>|<span data-ttu-id="c199f-121">Строка</span><span class="sxs-lookup"><span data-stu-id="c199f-121">String</span></span>|<span data-ttu-id="c199f-122">Отображение имени шаблона ссылаемого шаблона.</span><span class="sxs-lookup"><span data-stu-id="c199f-122">Template Display Name of the referenced template.</span></span> <span data-ttu-id="c199f-123">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c199f-123">This property is read-only.</span></span>|
|<span data-ttu-id="c199f-124">templateDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="c199f-124">templateDisplayVersion</span></span>|<span data-ttu-id="c199f-125">Строка</span><span class="sxs-lookup"><span data-stu-id="c199f-125">String</span></span>|<span data-ttu-id="c199f-126">Отображение шаблона версии ссылаемого шаблона.</span><span class="sxs-lookup"><span data-stu-id="c199f-126">Template Display Version of the referenced Template.</span></span> <span data-ttu-id="c199f-127">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c199f-127">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c199f-128">Связи</span><span class="sxs-lookup"><span data-stu-id="c199f-128">Relationships</span></span>
<span data-ttu-id="c199f-129">Нет</span><span class="sxs-lookup"><span data-stu-id="c199f-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c199f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c199f-130">JSON Representation</span></span>
<span data-ttu-id="c199f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c199f-131">Here is a JSON representation of the resource.</span></span>
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




