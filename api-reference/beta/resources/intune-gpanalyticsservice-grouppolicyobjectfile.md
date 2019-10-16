---
title: Тип ресурса Граупполициобжектфиле
description: Файл объекта групповой политики, переданный администратором.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b28ba6364f3261a7cd341870de402dc9332c87b4
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539199"
---
# <a name="grouppolicyobjectfile-resource-type"></a><span data-ttu-id="3e91d-103">Тип ресурса Граупполициобжектфиле</span><span class="sxs-lookup"><span data-stu-id="3e91d-103">groupPolicyObjectFile resource type</span></span>

> <span data-ttu-id="3e91d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e91d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e91d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e91d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e91d-106">Файл объекта групповой политики, переданный администратором.</span><span class="sxs-lookup"><span data-stu-id="3e91d-106">The Group Policy Object file uploaded by admin.</span></span>

## <a name="properties"></a><span data-ttu-id="3e91d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e91d-107">Properties</span></span>
|<span data-ttu-id="3e91d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e91d-108">Property</span></span>|<span data-ttu-id="3e91d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3e91d-109">Type</span></span>|<span data-ttu-id="3e91d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3e91d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e91d-111">аудистингуишеднаме</span><span class="sxs-lookup"><span data-stu-id="3e91d-111">ouDistinguishedName</span></span>|<span data-ttu-id="3e91d-112">String</span><span class="sxs-lookup"><span data-stu-id="3e91d-112">String</span></span>|<span data-ttu-id="3e91d-113">Различающееся имя подразделения.</span><span class="sxs-lookup"><span data-stu-id="3e91d-113">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="3e91d-114">content</span><span class="sxs-lookup"><span data-stu-id="3e91d-114">content</span></span>|<span data-ttu-id="3e91d-115">String</span><span class="sxs-lookup"><span data-stu-id="3e91d-115">String</span></span>|<span data-ttu-id="3e91d-116">Содержимое файла объекта групповой политики.</span><span class="sxs-lookup"><span data-stu-id="3e91d-116">The Group Policy Object file content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e91d-117">Связи</span><span class="sxs-lookup"><span data-stu-id="3e91d-117">Relationships</span></span>
<span data-ttu-id="3e91d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="3e91d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e91d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e91d-119">JSON Representation</span></span>
<span data-ttu-id="3e91d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e91d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "ouDistinguishedName": "String",
  "content": "String"
}
```



