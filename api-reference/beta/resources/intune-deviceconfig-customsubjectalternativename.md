---
title: Тип ресурса Кустомсубжекталтернативенаме
description: Определение альтернативного имени настраиваемой темы
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2d621b67cffcf676dcd35889907eb5f9ca34504
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729800"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="a5370-103">Тип ресурса Кустомсубжекталтернативенаме</span><span class="sxs-lookup"><span data-stu-id="a5370-103">customSubjectAlternativeName resource type</span></span>

<span data-ttu-id="a5370-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5370-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5370-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5370-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5370-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5370-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5370-107">Определение альтернативного имени настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="a5370-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="a5370-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5370-108">Properties</span></span>
|<span data-ttu-id="a5370-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5370-109">Property</span></span>|<span data-ttu-id="a5370-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a5370-110">Type</span></span>|<span data-ttu-id="a5370-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a5370-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5370-112">сантипе</span><span class="sxs-lookup"><span data-stu-id="a5370-112">sanType</span></span>|[<span data-ttu-id="a5370-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a5370-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a5370-114">Настраиваемый тип SAN.</span><span class="sxs-lookup"><span data-stu-id="a5370-114">Custom SAN Type.</span></span> <span data-ttu-id="a5370-115">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="a5370-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="a5370-116">name</span><span class="sxs-lookup"><span data-stu-id="a5370-116">name</span></span>|<span data-ttu-id="a5370-117">String</span><span class="sxs-lookup"><span data-stu-id="a5370-117">String</span></span>|<span data-ttu-id="a5370-118">Настраиваемое имя сети хранения данных</span><span class="sxs-lookup"><span data-stu-id="a5370-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5370-119">Связи</span><span class="sxs-lookup"><span data-stu-id="a5370-119">Relationships</span></span>
<span data-ttu-id="a5370-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a5370-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5370-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5370-121">JSON Representation</span></span>
<span data-ttu-id="a5370-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5370-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```





