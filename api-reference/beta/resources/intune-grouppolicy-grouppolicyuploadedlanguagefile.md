---
title: Тип ресурса Граупполициуплоадедлангуажефиле
description: Сущность представляет XML-файл ADML (язык административного шаблона), переданный администратором.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf5bef8faadac012df13a8a31cfaac3a5dc94ed2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298108"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a><span data-ttu-id="ab383-103">Тип ресурса Граупполициуплоадедлангуажефиле</span><span class="sxs-lookup"><span data-stu-id="ab383-103">groupPolicyUploadedLanguageFile resource type</span></span>

<span data-ttu-id="ab383-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab383-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab383-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab383-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab383-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab383-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab383-107">Сущность представляет XML-файл ADML (язык административного шаблона), переданный администратором.</span><span class="sxs-lookup"><span data-stu-id="ab383-107">The entity represents an ADML (Administrative Template language) XML file uploaded by Administrator.</span></span>

## <a name="properties"></a><span data-ttu-id="ab383-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab383-108">Properties</span></span>
|<span data-ttu-id="ab383-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab383-109">Property</span></span>|<span data-ttu-id="ab383-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ab383-110">Type</span></span>|<span data-ttu-id="ab383-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ab383-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab383-112">fileName</span><span class="sxs-lookup"><span data-stu-id="ab383-112">fileName</span></span>|<span data-ttu-id="ab383-113">String</span><span class="sxs-lookup"><span data-stu-id="ab383-113">String</span></span>|<span data-ttu-id="ab383-114">Имя файла загруженного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="ab383-114">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="ab383-115">лангуажекоде</span><span class="sxs-lookup"><span data-stu-id="ab383-115">languageCode</span></span>|<span data-ttu-id="ab383-116">String</span><span class="sxs-lookup"><span data-stu-id="ab383-116">String</span></span>|<span data-ttu-id="ab383-117">Код языка загруженного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="ab383-117">The language code of the uploaded ADML file.</span></span>|
|<span data-ttu-id="ab383-118">содержимое</span><span class="sxs-lookup"><span data-stu-id="ab383-118">content</span></span>|<span data-ttu-id="ab383-119">Binary</span><span class="sxs-lookup"><span data-stu-id="ab383-119">Binary</span></span>|<span data-ttu-id="ab383-120">Содержимое отправленного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="ab383-120">The contents of the uploaded ADML file.</span></span>|
|<span data-ttu-id="ab383-121">id</span><span class="sxs-lookup"><span data-stu-id="ab383-121">id</span></span>|<span data-ttu-id="ab383-122">String</span><span class="sxs-lookup"><span data-stu-id="ab383-122">String</span></span>|<span data-ttu-id="ab383-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ab383-123">Key of the entity.</span></span>|
|<span data-ttu-id="ab383-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab383-124">lastModifiedDateTime</span></span>|<span data-ttu-id="ab383-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab383-125">DateTimeOffset</span></span>|<span data-ttu-id="ab383-126">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ab383-126">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab383-127">Связи</span><span class="sxs-lookup"><span data-stu-id="ab383-127">Relationships</span></span>
<span data-ttu-id="ab383-128">Нет</span><span class="sxs-lookup"><span data-stu-id="ab383-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab383-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab383-129">JSON Representation</span></span>
<span data-ttu-id="ab383-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab383-130">Here is a JSON representation of the resource.</span></span>
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




