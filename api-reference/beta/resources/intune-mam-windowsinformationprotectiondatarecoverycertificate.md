---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5d755ed3b8a1bfb34df3702168abb3ad589474c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524267"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="2d60c-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="2d60c-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="2d60c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2d60c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d60c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d60c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d60c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d60c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d60c-107">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="2d60c-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="2d60c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d60c-108">Properties</span></span>
|<span data-ttu-id="2d60c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d60c-109">Property</span></span>|<span data-ttu-id="2d60c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2d60c-110">Type</span></span>|<span data-ttu-id="2d60c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2d60c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d60c-112">subjectName</span><span class="sxs-lookup"><span data-stu-id="2d60c-112">subjectName</span></span>|<span data-ttu-id="2d60c-113">String</span><span class="sxs-lookup"><span data-stu-id="2d60c-113">String</span></span>|<span data-ttu-id="2d60c-114">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="2d60c-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="2d60c-115">description</span><span class="sxs-lookup"><span data-stu-id="2d60c-115">description</span></span>|<span data-ttu-id="2d60c-116">String</span><span class="sxs-lookup"><span data-stu-id="2d60c-116">String</span></span>|<span data-ttu-id="2d60c-117">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="2d60c-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="2d60c-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2d60c-118">expirationDateTime</span></span>|<span data-ttu-id="2d60c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d60c-119">DateTimeOffset</span></span>|<span data-ttu-id="2d60c-120">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="2d60c-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="2d60c-121">certificate</span><span class="sxs-lookup"><span data-stu-id="2d60c-121">certificate</span></span>|<span data-ttu-id="2d60c-122">Двоичный</span><span class="sxs-lookup"><span data-stu-id="2d60c-122">Binary</span></span>|<span data-ttu-id="2d60c-123">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="2d60c-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d60c-124">Связи</span><span class="sxs-lookup"><span data-stu-id="2d60c-124">Relationships</span></span>
<span data-ttu-id="2d60c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="2d60c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d60c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d60c-126">JSON Representation</span></span>
<span data-ttu-id="2d60c-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d60c-127">Here is a JSON representation of the resource.</span></span>
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



