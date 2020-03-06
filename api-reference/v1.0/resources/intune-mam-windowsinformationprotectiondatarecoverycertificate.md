---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f49f5651c6e4f7bea1eb4650e9252c397cc2a930
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533324"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="75d29-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="75d29-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="75d29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75d29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75d29-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75d29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75d29-106">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="75d29-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="75d29-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="75d29-107">Properties</span></span>
|<span data-ttu-id="75d29-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="75d29-108">Property</span></span>|<span data-ttu-id="75d29-109">Тип</span><span class="sxs-lookup"><span data-stu-id="75d29-109">Type</span></span>|<span data-ttu-id="75d29-110">Описание</span><span class="sxs-lookup"><span data-stu-id="75d29-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75d29-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="75d29-111">subjectName</span></span>|<span data-ttu-id="75d29-112">String</span><span class="sxs-lookup"><span data-stu-id="75d29-112">String</span></span>|<span data-ttu-id="75d29-113">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="75d29-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="75d29-114">description</span><span class="sxs-lookup"><span data-stu-id="75d29-114">description</span></span>|<span data-ttu-id="75d29-115">String</span><span class="sxs-lookup"><span data-stu-id="75d29-115">String</span></span>|<span data-ttu-id="75d29-116">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="75d29-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="75d29-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="75d29-117">expirationDateTime</span></span>|<span data-ttu-id="75d29-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75d29-118">DateTimeOffset</span></span>|<span data-ttu-id="75d29-119">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="75d29-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="75d29-120">certificate</span><span class="sxs-lookup"><span data-stu-id="75d29-120">certificate</span></span>|<span data-ttu-id="75d29-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="75d29-121">Binary</span></span>|<span data-ttu-id="75d29-122">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="75d29-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="75d29-123">Связи</span><span class="sxs-lookup"><span data-stu-id="75d29-123">Relationships</span></span>
<span data-ttu-id="75d29-124">Нет</span><span class="sxs-lookup"><span data-stu-id="75d29-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75d29-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75d29-125">JSON Representation</span></span>
<span data-ttu-id="75d29-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75d29-126">Here is a JSON representation of the resource.</span></span>
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




