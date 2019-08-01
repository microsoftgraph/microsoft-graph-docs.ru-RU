---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 555cac098d2796f612054f11e2c5ade525ad6199
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037732"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="59a5c-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="59a5c-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="59a5c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59a5c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59a5c-105">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="59a5c-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="59a5c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="59a5c-106">Properties</span></span>
|<span data-ttu-id="59a5c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="59a5c-107">Property</span></span>|<span data-ttu-id="59a5c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="59a5c-108">Type</span></span>|<span data-ttu-id="59a5c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59a5c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59a5c-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="59a5c-110">subjectName</span></span>|<span data-ttu-id="59a5c-111">String</span><span class="sxs-lookup"><span data-stu-id="59a5c-111">String</span></span>|<span data-ttu-id="59a5c-112">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="59a5c-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="59a5c-113">description</span><span class="sxs-lookup"><span data-stu-id="59a5c-113">description</span></span>|<span data-ttu-id="59a5c-114">String</span><span class="sxs-lookup"><span data-stu-id="59a5c-114">String</span></span>|<span data-ttu-id="59a5c-115">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="59a5c-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="59a5c-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="59a5c-116">expirationDateTime</span></span>|<span data-ttu-id="59a5c-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59a5c-117">DateTimeOffset</span></span>|<span data-ttu-id="59a5c-118">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="59a5c-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="59a5c-119">certificate</span><span class="sxs-lookup"><span data-stu-id="59a5c-119">certificate</span></span>|<span data-ttu-id="59a5c-120">Двоичный</span><span class="sxs-lookup"><span data-stu-id="59a5c-120">Binary</span></span>|<span data-ttu-id="59a5c-121">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="59a5c-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="59a5c-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="59a5c-122">Relationships</span></span>
<span data-ttu-id="59a5c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="59a5c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59a5c-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59a5c-124">JSON Representation</span></span>
<span data-ttu-id="59a5c-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59a5c-125">Here is a JSON representation of the resource.</span></span>
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



