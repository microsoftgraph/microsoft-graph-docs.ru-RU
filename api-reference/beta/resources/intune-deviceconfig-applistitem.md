---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b32e08474296894e2bb54135f6daab347b6fb7fa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260812"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="60f72-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="60f72-103">appListItem resource type</span></span>

<span data-ttu-id="60f72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60f72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60f72-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60f72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60f72-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60f72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60f72-107">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="60f72-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="60f72-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="60f72-108">Properties</span></span>
|<span data-ttu-id="60f72-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="60f72-109">Property</span></span>|<span data-ttu-id="60f72-110">Тип</span><span class="sxs-lookup"><span data-stu-id="60f72-110">Type</span></span>|<span data-ttu-id="60f72-111">Описание</span><span class="sxs-lookup"><span data-stu-id="60f72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60f72-112">name</span><span class="sxs-lookup"><span data-stu-id="60f72-112">name</span></span>|<span data-ttu-id="60f72-113">String</span><span class="sxs-lookup"><span data-stu-id="60f72-113">String</span></span>|<span data-ttu-id="60f72-114">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="60f72-114">The application name</span></span>|
|<span data-ttu-id="60f72-115">publisher</span><span class="sxs-lookup"><span data-stu-id="60f72-115">publisher</span></span>|<span data-ttu-id="60f72-116">String</span><span class="sxs-lookup"><span data-stu-id="60f72-116">String</span></span>|<span data-ttu-id="60f72-117">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="60f72-117">The publisher of the application</span></span>|
|<span data-ttu-id="60f72-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="60f72-118">appStoreUrl</span></span>|<span data-ttu-id="60f72-119">String</span><span class="sxs-lookup"><span data-stu-id="60f72-119">String</span></span>|<span data-ttu-id="60f72-120">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="60f72-120">The Store URL of the application</span></span>|
|<span data-ttu-id="60f72-121">appId</span><span class="sxs-lookup"><span data-stu-id="60f72-121">appId</span></span>|<span data-ttu-id="60f72-122">String</span><span class="sxs-lookup"><span data-stu-id="60f72-122">String</span></span>|<span data-ttu-id="60f72-123">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="60f72-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="60f72-124">Связи</span><span class="sxs-lookup"><span data-stu-id="60f72-124">Relationships</span></span>
<span data-ttu-id="60f72-125">Нет</span><span class="sxs-lookup"><span data-stu-id="60f72-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60f72-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60f72-126">JSON Representation</span></span>
<span data-ttu-id="60f72-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60f72-127">Here is a JSON representation of the resource.</span></span>
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




