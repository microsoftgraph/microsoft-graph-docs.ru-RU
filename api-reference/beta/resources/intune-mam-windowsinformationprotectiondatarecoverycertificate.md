---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 272a1e5f7bf1df1c9e16b2239caeee94cc81f12d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790636"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="71ee1-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="71ee1-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="71ee1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71ee1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71ee1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71ee1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71ee1-106">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="71ee1-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="71ee1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="71ee1-107">Properties</span></span>
|<span data-ttu-id="71ee1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="71ee1-108">Property</span></span>|<span data-ttu-id="71ee1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="71ee1-109">Type</span></span>|<span data-ttu-id="71ee1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="71ee1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71ee1-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="71ee1-111">subjectName</span></span>|<span data-ttu-id="71ee1-112">String</span><span class="sxs-lookup"><span data-stu-id="71ee1-112">String</span></span>|<span data-ttu-id="71ee1-113">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="71ee1-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="71ee1-114">description</span><span class="sxs-lookup"><span data-stu-id="71ee1-114">description</span></span>|<span data-ttu-id="71ee1-115">String</span><span class="sxs-lookup"><span data-stu-id="71ee1-115">String</span></span>|<span data-ttu-id="71ee1-116">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="71ee1-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="71ee1-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="71ee1-117">expirationDateTime</span></span>|<span data-ttu-id="71ee1-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71ee1-118">DateTimeOffset</span></span>|<span data-ttu-id="71ee1-119">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="71ee1-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="71ee1-120">certificate</span><span class="sxs-lookup"><span data-stu-id="71ee1-120">certificate</span></span>|<span data-ttu-id="71ee1-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="71ee1-121">Binary</span></span>|<span data-ttu-id="71ee1-122">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="71ee1-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="71ee1-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="71ee1-123">Relationships</span></span>
<span data-ttu-id="71ee1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="71ee1-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71ee1-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71ee1-125">JSON Representation</span></span>
<span data-ttu-id="71ee1-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71ee1-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```





