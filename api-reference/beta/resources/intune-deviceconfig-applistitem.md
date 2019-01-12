---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 492828fdef95815704083ec8f496e38a10dc3559
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923336"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="ecc1a-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="ecc1a-103">appListItem resource type</span></span>

> <span data-ttu-id="ecc1a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ecc1a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecc1a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecc1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecc1a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ecc1a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecc1a-107">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="ecc1a-107">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="ecc1a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ecc1a-108">Properties</span></span>
|<span data-ttu-id="ecc1a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecc1a-109">Property</span></span>|<span data-ttu-id="ecc1a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ecc1a-110">Type</span></span>|<span data-ttu-id="ecc1a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ecc1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecc1a-112">name</span><span class="sxs-lookup"><span data-stu-id="ecc1a-112">name</span></span>|<span data-ttu-id="ecc1a-113">String</span><span class="sxs-lookup"><span data-stu-id="ecc1a-113">String</span></span>|<span data-ttu-id="ecc1a-114">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="ecc1a-114">The application name</span></span>|
|<span data-ttu-id="ecc1a-115">publisher</span><span class="sxs-lookup"><span data-stu-id="ecc1a-115">publisher</span></span>|<span data-ttu-id="ecc1a-116">String</span><span class="sxs-lookup"><span data-stu-id="ecc1a-116">String</span></span>|<span data-ttu-id="ecc1a-117">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="ecc1a-117">The publisher of the application</span></span>|
|<span data-ttu-id="ecc1a-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ecc1a-118">appStoreUrl</span></span>|<span data-ttu-id="ecc1a-119">String</span><span class="sxs-lookup"><span data-stu-id="ecc1a-119">String</span></span>|<span data-ttu-id="ecc1a-120">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="ecc1a-120">The Store URL of the application</span></span>|
|<span data-ttu-id="ecc1a-121">appId</span><span class="sxs-lookup"><span data-stu-id="ecc1a-121">appId</span></span>|<span data-ttu-id="ecc1a-122">String</span><span class="sxs-lookup"><span data-stu-id="ecc1a-122">String</span></span>|<span data-ttu-id="ecc1a-123">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="ecc1a-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecc1a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="ecc1a-124">Relationships</span></span>
<span data-ttu-id="ecc1a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="ecc1a-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ecc1a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ecc1a-126">JSON Representation</span></span>
<span data-ttu-id="ecc1a-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecc1a-127">Here is a JSON representation of the resource.</span></span>
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





