---
title: Тип ресурса МакосассоЦиатеддомаинситем
description: Сопоставление идентификаторов приложений со связанными доменами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fa40fda83eb6dd89fa0d8fd709a8bf744a8cc19
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736256"
---
# <a name="macosassociateddomainsitem-resource-type"></a><span data-ttu-id="6a912-103">Тип ресурса МакосассоЦиатеддомаинситем</span><span class="sxs-lookup"><span data-stu-id="6a912-103">macOSAssociatedDomainsItem resource type</span></span>

<span data-ttu-id="6a912-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a912-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a912-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a912-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a912-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a912-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a912-107">Сопоставление идентификаторов приложений со связанными доменами.</span><span class="sxs-lookup"><span data-stu-id="6a912-107">A mapping of application identifiers to associated domains.</span></span>

## <a name="properties"></a><span data-ttu-id="6a912-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a912-108">Properties</span></span>
|<span data-ttu-id="6a912-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a912-109">Property</span></span>|<span data-ttu-id="6a912-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6a912-110">Type</span></span>|<span data-ttu-id="6a912-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6a912-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a912-112">applicationIdentifier</span><span class="sxs-lookup"><span data-stu-id="6a912-112">applicationIdentifier</span></span>|<span data-ttu-id="6a912-113">Строка</span><span class="sxs-lookup"><span data-stu-id="6a912-113">String</span></span>|<span data-ttu-id="6a912-114">Идентификатор приложения, с которым связываются домены.</span><span class="sxs-lookup"><span data-stu-id="6a912-114">The application identifier of the app to associate domains with.</span></span>|
|<span data-ttu-id="6a912-115">домена</span><span class="sxs-lookup"><span data-stu-id="6a912-115">domains</span></span>|<span data-ttu-id="6a912-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6a912-116">String collection</span></span>|<span data-ttu-id="6a912-117">Список подсвязываемых доменов.</span><span class="sxs-lookup"><span data-stu-id="6a912-117">The list of domains to associate.</span></span>|
|<span data-ttu-id="6a912-118">директдовнлоадсенаблед</span><span class="sxs-lookup"><span data-stu-id="6a912-118">directDownloadsEnabled</span></span>|<span data-ttu-id="6a912-119">Логический</span><span class="sxs-lookup"><span data-stu-id="6a912-119">Boolean</span></span>|<span data-ttu-id="6a912-120">Определяет, будут ли данные загружаться напрямую или с помощью сети CDN.</span><span class="sxs-lookup"><span data-stu-id="6a912-120">Determines whether data should be downloaded directly or via a CDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a912-121">Связи</span><span class="sxs-lookup"><span data-stu-id="6a912-121">Relationships</span></span>
<span data-ttu-id="6a912-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6a912-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a912-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a912-123">JSON Representation</span></span>
<span data-ttu-id="6a912-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a912-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsItem",
  "applicationIdentifier": "String",
  "domains": [
    "String"
  ],
  "directDownloadsEnabled": true
}
```





