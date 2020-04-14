---
title: Тип ресурса Граупполициуплоадедлангуажефиле
description: Сущность представляет XML-файл ADML (язык административного шаблона), переданный администратором.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c3b2a4fd4ab035dd072af8db0cd6897bfd7d9153
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385904"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a><span data-ttu-id="358fe-103">Тип ресурса Граупполициуплоадедлангуажефиле</span><span class="sxs-lookup"><span data-stu-id="358fe-103">groupPolicyUploadedLanguageFile resource type</span></span>

<span data-ttu-id="358fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="358fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="358fe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="358fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="358fe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="358fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="358fe-107">Сущность представляет XML-файл ADML (язык административного шаблона), переданный администратором.</span><span class="sxs-lookup"><span data-stu-id="358fe-107">The entity represents an ADML (Administrative Template language) XML file uploaded by Administrator.</span></span>

## <a name="properties"></a><span data-ttu-id="358fe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="358fe-108">Properties</span></span>
|<span data-ttu-id="358fe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="358fe-109">Property</span></span>|<span data-ttu-id="358fe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="358fe-110">Type</span></span>|<span data-ttu-id="358fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="358fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="358fe-112">fileName</span><span class="sxs-lookup"><span data-stu-id="358fe-112">fileName</span></span>|<span data-ttu-id="358fe-113">String</span><span class="sxs-lookup"><span data-stu-id="358fe-113">String</span></span>|<span data-ttu-id="358fe-114">Имя файла загруженного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="358fe-114">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="358fe-115">лангуажекоде</span><span class="sxs-lookup"><span data-stu-id="358fe-115">languageCode</span></span>|<span data-ttu-id="358fe-116">String</span><span class="sxs-lookup"><span data-stu-id="358fe-116">String</span></span>|<span data-ttu-id="358fe-117">Код языка загруженного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="358fe-117">The language code of the uploaded ADML file.</span></span>|
|<span data-ttu-id="358fe-118">содержимое</span><span class="sxs-lookup"><span data-stu-id="358fe-118">content</span></span>|<span data-ttu-id="358fe-119">Binary</span><span class="sxs-lookup"><span data-stu-id="358fe-119">Binary</span></span>|<span data-ttu-id="358fe-120">Содержимое отправленного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="358fe-120">The contents of the uploaded ADML file.</span></span>|
|<span data-ttu-id="358fe-121">id</span><span class="sxs-lookup"><span data-stu-id="358fe-121">id</span></span>|<span data-ttu-id="358fe-122">String</span><span class="sxs-lookup"><span data-stu-id="358fe-122">String</span></span>|<span data-ttu-id="358fe-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="358fe-123">Key of the entity.</span></span>|
|<span data-ttu-id="358fe-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="358fe-124">lastModifiedDateTime</span></span>|<span data-ttu-id="358fe-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="358fe-125">DateTimeOffset</span></span>|<span data-ttu-id="358fe-126">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="358fe-126">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="358fe-127">Связи</span><span class="sxs-lookup"><span data-stu-id="358fe-127">Relationships</span></span>
<span data-ttu-id="358fe-128">Нет</span><span class="sxs-lookup"><span data-stu-id="358fe-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="358fe-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="358fe-129">JSON Representation</span></span>
<span data-ttu-id="358fe-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="358fe-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedLanguageFile",
  "fileName": "String",
  "languageCode": "String",
  "content": "binary",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



