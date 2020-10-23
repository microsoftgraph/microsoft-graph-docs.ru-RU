---
title: Тип ресурса Граупполициуплоадедлангуажефиле
description: Сущность представляет XML-файл ADML (язык административного шаблона), переданный администратором.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc70d0ff85cebc567b9efc67b87bb57e2e8337fa
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707691"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a><span data-ttu-id="72a8d-103">Тип ресурса Граупполициуплоадедлангуажефиле</span><span class="sxs-lookup"><span data-stu-id="72a8d-103">groupPolicyUploadedLanguageFile resource type</span></span>

<span data-ttu-id="72a8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72a8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72a8d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72a8d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72a8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72a8d-107">Сущность представляет XML-файл ADML (язык административного шаблона), переданный администратором.</span><span class="sxs-lookup"><span data-stu-id="72a8d-107">The entity represents an ADML (Administrative Template language) XML file uploaded by Administrator.</span></span>

## <a name="properties"></a><span data-ttu-id="72a8d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="72a8d-108">Properties</span></span>
|<span data-ttu-id="72a8d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="72a8d-109">Property</span></span>|<span data-ttu-id="72a8d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="72a8d-110">Type</span></span>|<span data-ttu-id="72a8d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="72a8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72a8d-112">fileName</span><span class="sxs-lookup"><span data-stu-id="72a8d-112">fileName</span></span>|<span data-ttu-id="72a8d-113">String</span><span class="sxs-lookup"><span data-stu-id="72a8d-113">String</span></span>|<span data-ttu-id="72a8d-114">Имя файла загруженного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="72a8d-114">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="72a8d-115">лангуажекоде</span><span class="sxs-lookup"><span data-stu-id="72a8d-115">languageCode</span></span>|<span data-ttu-id="72a8d-116">Строка</span><span class="sxs-lookup"><span data-stu-id="72a8d-116">String</span></span>|<span data-ttu-id="72a8d-117">Код языка загруженного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="72a8d-117">The language code of the uploaded ADML file.</span></span>|
|<span data-ttu-id="72a8d-118">содержимое</span><span class="sxs-lookup"><span data-stu-id="72a8d-118">content</span></span>|<span data-ttu-id="72a8d-119">Binary</span><span class="sxs-lookup"><span data-stu-id="72a8d-119">Binary</span></span>|<span data-ttu-id="72a8d-120">Содержимое отправленного файла ADML.</span><span class="sxs-lookup"><span data-stu-id="72a8d-120">The contents of the uploaded ADML file.</span></span>|
|<span data-ttu-id="72a8d-121">id</span><span class="sxs-lookup"><span data-stu-id="72a8d-121">id</span></span>|<span data-ttu-id="72a8d-122">Строка</span><span class="sxs-lookup"><span data-stu-id="72a8d-122">String</span></span>|<span data-ttu-id="72a8d-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72a8d-123">Key of the entity.</span></span>|
|<span data-ttu-id="72a8d-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72a8d-124">lastModifiedDateTime</span></span>|<span data-ttu-id="72a8d-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72a8d-125">DateTimeOffset</span></span>|<span data-ttu-id="72a8d-126">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="72a8d-126">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72a8d-127">Связи</span><span class="sxs-lookup"><span data-stu-id="72a8d-127">Relationships</span></span>
<span data-ttu-id="72a8d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="72a8d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72a8d-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72a8d-129">JSON Representation</span></span>
<span data-ttu-id="72a8d-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72a8d-130">Here is a JSON representation of the resource.</span></span>
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





