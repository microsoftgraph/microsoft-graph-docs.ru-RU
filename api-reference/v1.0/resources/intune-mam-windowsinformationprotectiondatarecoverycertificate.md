---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a62c0351b3247300e47c8c9a91aecbc32092e015
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367324"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="8bf9d-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8bf9d-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="8bf9d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bf9d-105">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="8bf9d-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="8bf9d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bf9d-106">Properties</span></span>
|<span data-ttu-id="8bf9d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bf9d-107">Property</span></span>|<span data-ttu-id="8bf9d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8bf9d-108">Type</span></span>|<span data-ttu-id="8bf9d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8bf9d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bf9d-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="8bf9d-110">subjectName</span></span>|<span data-ttu-id="8bf9d-111">String</span><span class="sxs-lookup"><span data-stu-id="8bf9d-111">String</span></span>|<span data-ttu-id="8bf9d-112">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8bf9d-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="8bf9d-113">description</span><span class="sxs-lookup"><span data-stu-id="8bf9d-113">description</span></span>|<span data-ttu-id="8bf9d-114">String</span><span class="sxs-lookup"><span data-stu-id="8bf9d-114">String</span></span>|<span data-ttu-id="8bf9d-115">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8bf9d-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="8bf9d-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8bf9d-116">expirationDateTime</span></span>|<span data-ttu-id="8bf9d-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bf9d-117">DateTimeOffset</span></span>|<span data-ttu-id="8bf9d-118">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8bf9d-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="8bf9d-119">certificate</span><span class="sxs-lookup"><span data-stu-id="8bf9d-119">certificate</span></span>|<span data-ttu-id="8bf9d-120">Двоичный</span><span class="sxs-lookup"><span data-stu-id="8bf9d-120">Binary</span></span>|<span data-ttu-id="8bf9d-121">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8bf9d-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bf9d-122">Связи</span><span class="sxs-lookup"><span data-stu-id="8bf9d-122">Relationships</span></span>
<span data-ttu-id="8bf9d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="8bf9d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bf9d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bf9d-124">JSON Representation</span></span>
<span data-ttu-id="8bf9d-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bf9d-125">Here is a JSON representation of the resource.</span></span>
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




