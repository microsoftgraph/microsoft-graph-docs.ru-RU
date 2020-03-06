---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: acb27cacd61685c36043789b25f70f015d1fe0b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530931"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="0bda3-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="0bda3-103">appListItem resource type</span></span>

<span data-ttu-id="0bda3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bda3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bda3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bda3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bda3-106">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="0bda3-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="0bda3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bda3-107">Properties</span></span>
|<span data-ttu-id="0bda3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bda3-108">Property</span></span>|<span data-ttu-id="0bda3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0bda3-109">Type</span></span>|<span data-ttu-id="0bda3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0bda3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bda3-111">name</span><span class="sxs-lookup"><span data-stu-id="0bda3-111">name</span></span>|<span data-ttu-id="0bda3-112">Строка</span><span class="sxs-lookup"><span data-stu-id="0bda3-112">String</span></span>|<span data-ttu-id="0bda3-113">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="0bda3-113">The application name</span></span>|
|<span data-ttu-id="0bda3-114">publisher</span><span class="sxs-lookup"><span data-stu-id="0bda3-114">publisher</span></span>|<span data-ttu-id="0bda3-115">Строка</span><span class="sxs-lookup"><span data-stu-id="0bda3-115">String</span></span>|<span data-ttu-id="0bda3-116">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="0bda3-116">The publisher of the application</span></span>|
|<span data-ttu-id="0bda3-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0bda3-117">appStoreUrl</span></span>|<span data-ttu-id="0bda3-118">String</span><span class="sxs-lookup"><span data-stu-id="0bda3-118">String</span></span>|<span data-ttu-id="0bda3-119">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="0bda3-119">The Store URL of the application</span></span>|
|<span data-ttu-id="0bda3-120">appId</span><span class="sxs-lookup"><span data-stu-id="0bda3-120">appId</span></span>|<span data-ttu-id="0bda3-121">String</span><span class="sxs-lookup"><span data-stu-id="0bda3-121">String</span></span>|<span data-ttu-id="0bda3-122">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="0bda3-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bda3-123">Связи</span><span class="sxs-lookup"><span data-stu-id="0bda3-123">Relationships</span></span>
<span data-ttu-id="0bda3-124">Нет</span><span class="sxs-lookup"><span data-stu-id="0bda3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bda3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0bda3-125">JSON Representation</span></span>
<span data-ttu-id="0bda3-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bda3-126">Here is a JSON representation of the resource.</span></span>
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




