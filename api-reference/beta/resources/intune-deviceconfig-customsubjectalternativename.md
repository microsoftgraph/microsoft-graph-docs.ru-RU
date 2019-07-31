---
title: Тип ресурса Кустомсубжекталтернативенаме
description: Определение альтернативного имени настраиваемой темы
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ac276e4167700afb6608eba27e72f76db0fd34f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001798"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="ab032-103">Тип ресурса Кустомсубжекталтернативенаме</span><span class="sxs-lookup"><span data-stu-id="ab032-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="ab032-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab032-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab032-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab032-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab032-106">Определение альтернативного имени настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="ab032-106">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="ab032-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab032-107">Properties</span></span>
|<span data-ttu-id="ab032-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab032-108">Property</span></span>|<span data-ttu-id="ab032-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ab032-109">Type</span></span>|<span data-ttu-id="ab032-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ab032-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab032-111">Сантипе</span><span class="sxs-lookup"><span data-stu-id="ab032-111">sanType</span></span>|[<span data-ttu-id="ab032-112">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ab032-112">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ab032-113">Настраиваемый тип SAN.</span><span class="sxs-lookup"><span data-stu-id="ab032-113">Custom SAN Type.</span></span> <span data-ttu-id="ab032-114">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="ab032-114">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ab032-115">name</span><span class="sxs-lookup"><span data-stu-id="ab032-115">name</span></span>|<span data-ttu-id="ab032-116">String</span><span class="sxs-lookup"><span data-stu-id="ab032-116">String</span></span>|<span data-ttu-id="ab032-117">Настраиваемое имя сети хранения данных</span><span class="sxs-lookup"><span data-stu-id="ab032-117">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab032-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="ab032-118">Relationships</span></span>
<span data-ttu-id="ab032-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ab032-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab032-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab032-120">JSON Representation</span></span>
<span data-ttu-id="ab032-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab032-121">Here is a JSON representation of the resource.</span></span>
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





