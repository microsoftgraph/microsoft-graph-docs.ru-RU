---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9571b622fc098f384f7c3a6c62b1d1e10d89f663
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405417"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="3c221-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="3c221-103">appListItem resource type</span></span>

> <span data-ttu-id="3c221-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c221-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3c221-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c221-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c221-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c221-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c221-107">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="3c221-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="3c221-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c221-108">Properties</span></span>
|<span data-ttu-id="3c221-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c221-109">Property</span></span>|<span data-ttu-id="3c221-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3c221-110">Type</span></span>|<span data-ttu-id="3c221-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3c221-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c221-112">name</span><span class="sxs-lookup"><span data-stu-id="3c221-112">name</span></span>|<span data-ttu-id="3c221-113">String</span><span class="sxs-lookup"><span data-stu-id="3c221-113">String</span></span>|<span data-ttu-id="3c221-114">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="3c221-114">The application name</span></span>|
|<span data-ttu-id="3c221-115">publisher</span><span class="sxs-lookup"><span data-stu-id="3c221-115">publisher</span></span>|<span data-ttu-id="3c221-116">String</span><span class="sxs-lookup"><span data-stu-id="3c221-116">String</span></span>|<span data-ttu-id="3c221-117">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="3c221-117">The publisher of the application</span></span>|
|<span data-ttu-id="3c221-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3c221-118">appStoreUrl</span></span>|<span data-ttu-id="3c221-119">String</span><span class="sxs-lookup"><span data-stu-id="3c221-119">String</span></span>|<span data-ttu-id="3c221-120">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="3c221-120">The Store URL of the application</span></span>|
|<span data-ttu-id="3c221-121">appId</span><span class="sxs-lookup"><span data-stu-id="3c221-121">appId</span></span>|<span data-ttu-id="3c221-122">String</span><span class="sxs-lookup"><span data-stu-id="3c221-122">String</span></span>|<span data-ttu-id="3c221-123">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="3c221-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c221-124">Связи</span><span class="sxs-lookup"><span data-stu-id="3c221-124">Relationships</span></span>
<span data-ttu-id="3c221-125">Нет</span><span class="sxs-lookup"><span data-stu-id="3c221-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c221-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c221-126">JSON Representation</span></span>
<span data-ttu-id="3c221-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c221-127">Here is a JSON representation of the resource.</span></span>
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




