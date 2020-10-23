---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4ad031e97d6511280517ef1e9c3b30141c7125c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727190"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="ccea3-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="ccea3-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="ccea3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccea3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccea3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccea3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccea3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccea3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccea3-107">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="ccea3-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="ccea3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ccea3-108">Properties</span></span>
|<span data-ttu-id="ccea3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccea3-109">Property</span></span>|<span data-ttu-id="ccea3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ccea3-110">Type</span></span>|<span data-ttu-id="ccea3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ccea3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccea3-112">subjectName</span><span class="sxs-lookup"><span data-stu-id="ccea3-112">subjectName</span></span>|<span data-ttu-id="ccea3-113">String</span><span class="sxs-lookup"><span data-stu-id="ccea3-113">String</span></span>|<span data-ttu-id="ccea3-114">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="ccea3-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="ccea3-115">description</span><span class="sxs-lookup"><span data-stu-id="ccea3-115">description</span></span>|<span data-ttu-id="ccea3-116">Строка</span><span class="sxs-lookup"><span data-stu-id="ccea3-116">String</span></span>|<span data-ttu-id="ccea3-117">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="ccea3-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="ccea3-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ccea3-118">expirationDateTime</span></span>|<span data-ttu-id="ccea3-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccea3-119">DateTimeOffset</span></span>|<span data-ttu-id="ccea3-120">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="ccea3-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="ccea3-121">certificate</span><span class="sxs-lookup"><span data-stu-id="ccea3-121">certificate</span></span>|<span data-ttu-id="ccea3-122">Двоичный</span><span class="sxs-lookup"><span data-stu-id="ccea3-122">Binary</span></span>|<span data-ttu-id="ccea3-123">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="ccea3-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccea3-124">Связи</span><span class="sxs-lookup"><span data-stu-id="ccea3-124">Relationships</span></span>
<span data-ttu-id="ccea3-125">Нет</span><span class="sxs-lookup"><span data-stu-id="ccea3-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccea3-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ccea3-126">JSON Representation</span></span>
<span data-ttu-id="ccea3-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccea3-127">Here is a JSON representation of the resource.</span></span>
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





