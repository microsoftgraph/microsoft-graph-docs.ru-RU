---
title: Тип ресурса Граупполициобжектфиле
description: Файл объекта групповой политики, переданный администратором.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26881a87b7f22510acf760ae04f967db021e8730
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524478"
---
# <a name="grouppolicyobjectfile-resource-type"></a><span data-ttu-id="a7b5d-103">Тип ресурса Граупполициобжектфиле</span><span class="sxs-lookup"><span data-stu-id="a7b5d-103">groupPolicyObjectFile resource type</span></span>

<span data-ttu-id="a7b5d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a7b5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7b5d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7b5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7b5d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7b5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7b5d-107">Файл объекта групповой политики, переданный администратором.</span><span class="sxs-lookup"><span data-stu-id="a7b5d-107">The Group Policy Object file uploaded by admin.</span></span>

## <a name="properties"></a><span data-ttu-id="a7b5d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7b5d-108">Properties</span></span>
|<span data-ttu-id="a7b5d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7b5d-109">Property</span></span>|<span data-ttu-id="a7b5d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a7b5d-110">Type</span></span>|<span data-ttu-id="a7b5d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a7b5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7b5d-112">аудистингуишеднаме</span><span class="sxs-lookup"><span data-stu-id="a7b5d-112">ouDistinguishedName</span></span>|<span data-ttu-id="a7b5d-113">String</span><span class="sxs-lookup"><span data-stu-id="a7b5d-113">String</span></span>|<span data-ttu-id="a7b5d-114">Различающееся имя подразделения.</span><span class="sxs-lookup"><span data-stu-id="a7b5d-114">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="a7b5d-115">content</span><span class="sxs-lookup"><span data-stu-id="a7b5d-115">content</span></span>|<span data-ttu-id="a7b5d-116">String</span><span class="sxs-lookup"><span data-stu-id="a7b5d-116">String</span></span>|<span data-ttu-id="a7b5d-117">Содержимое файла объекта групповой политики.</span><span class="sxs-lookup"><span data-stu-id="a7b5d-117">The Group Policy Object file content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7b5d-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a7b5d-118">Relationships</span></span>
<span data-ttu-id="a7b5d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a7b5d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7b5d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7b5d-120">JSON Representation</span></span>
<span data-ttu-id="a7b5d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7b5d-121">Here is a JSON representation of the resource.</span></span>
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



