---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ccf980b0874ea40989eb297abd6bbf455e827f95
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708832"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="709ef-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="709ef-103">appListItem resource type</span></span>

<span data-ttu-id="709ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="709ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="709ef-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="709ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="709ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="709ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="709ef-107">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="709ef-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="709ef-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="709ef-108">Properties</span></span>
|<span data-ttu-id="709ef-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="709ef-109">Property</span></span>|<span data-ttu-id="709ef-110">Тип</span><span class="sxs-lookup"><span data-stu-id="709ef-110">Type</span></span>|<span data-ttu-id="709ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="709ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="709ef-112">name</span><span class="sxs-lookup"><span data-stu-id="709ef-112">name</span></span>|<span data-ttu-id="709ef-113">String</span><span class="sxs-lookup"><span data-stu-id="709ef-113">String</span></span>|<span data-ttu-id="709ef-114">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="709ef-114">The application name</span></span>|
|<span data-ttu-id="709ef-115">publisher</span><span class="sxs-lookup"><span data-stu-id="709ef-115">publisher</span></span>|<span data-ttu-id="709ef-116">String</span><span class="sxs-lookup"><span data-stu-id="709ef-116">String</span></span>|<span data-ttu-id="709ef-117">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="709ef-117">The publisher of the application</span></span>|
|<span data-ttu-id="709ef-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="709ef-118">appStoreUrl</span></span>|<span data-ttu-id="709ef-119">String</span><span class="sxs-lookup"><span data-stu-id="709ef-119">String</span></span>|<span data-ttu-id="709ef-120">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="709ef-120">The Store URL of the application</span></span>|
|<span data-ttu-id="709ef-121">appId</span><span class="sxs-lookup"><span data-stu-id="709ef-121">appId</span></span>|<span data-ttu-id="709ef-122">String</span><span class="sxs-lookup"><span data-stu-id="709ef-122">String</span></span>|<span data-ttu-id="709ef-123">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="709ef-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="709ef-124">Связи</span><span class="sxs-lookup"><span data-stu-id="709ef-124">Relationships</span></span>
<span data-ttu-id="709ef-125">Нет</span><span class="sxs-lookup"><span data-stu-id="709ef-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="709ef-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="709ef-126">JSON Representation</span></span>
<span data-ttu-id="709ef-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="709ef-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```





