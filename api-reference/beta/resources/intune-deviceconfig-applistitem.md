---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6a6eb9922accf3eb59ecd8e8b0c31edc7fa7e99
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987588"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="b22df-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="b22df-103">appListItem resource type</span></span>

> <span data-ttu-id="b22df-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b22df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b22df-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b22df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b22df-106">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="b22df-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="b22df-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b22df-107">Properties</span></span>
|<span data-ttu-id="b22df-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b22df-108">Property</span></span>|<span data-ttu-id="b22df-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b22df-109">Type</span></span>|<span data-ttu-id="b22df-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b22df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b22df-111">name</span><span class="sxs-lookup"><span data-stu-id="b22df-111">name</span></span>|<span data-ttu-id="b22df-112">Строка</span><span class="sxs-lookup"><span data-stu-id="b22df-112">String</span></span>|<span data-ttu-id="b22df-113">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="b22df-113">The application name</span></span>|
|<span data-ttu-id="b22df-114">publisher</span><span class="sxs-lookup"><span data-stu-id="b22df-114">publisher</span></span>|<span data-ttu-id="b22df-115">String</span><span class="sxs-lookup"><span data-stu-id="b22df-115">String</span></span>|<span data-ttu-id="b22df-116">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="b22df-116">The publisher of the application</span></span>|
|<span data-ttu-id="b22df-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b22df-117">appStoreUrl</span></span>|<span data-ttu-id="b22df-118">String</span><span class="sxs-lookup"><span data-stu-id="b22df-118">String</span></span>|<span data-ttu-id="b22df-119">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="b22df-119">The Store URL of the application</span></span>|
|<span data-ttu-id="b22df-120">appId</span><span class="sxs-lookup"><span data-stu-id="b22df-120">appId</span></span>|<span data-ttu-id="b22df-121">String</span><span class="sxs-lookup"><span data-stu-id="b22df-121">String</span></span>|<span data-ttu-id="b22df-122">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="b22df-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="b22df-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="b22df-123">Relationships</span></span>
<span data-ttu-id="b22df-124">Нет</span><span class="sxs-lookup"><span data-stu-id="b22df-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b22df-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b22df-125">JSON Representation</span></span>
<span data-ttu-id="b22df-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b22df-126">Here is a JSON representation of the resource.</span></span>
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





