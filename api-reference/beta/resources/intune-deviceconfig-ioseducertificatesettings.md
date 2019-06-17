---
title: Тип ресурса Иоседуцертификатесеттингс
description: Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30e7a68f76c60fafff9fc2b035a65a60307f775d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981470"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="69602-103">Тип ресурса Иоседуцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="69602-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="69602-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69602-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69602-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69602-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69602-106">Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="69602-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="69602-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="69602-107">Properties</span></span>
|<span data-ttu-id="69602-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="69602-108">Property</span></span>|<span data-ttu-id="69602-109">Тип</span><span class="sxs-lookup"><span data-stu-id="69602-109">Type</span></span>|<span data-ttu-id="69602-110">Описание</span><span class="sxs-lookup"><span data-stu-id="69602-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69602-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="69602-111">trustedRootCertificate</span></span>|<span data-ttu-id="69602-112">Binary</span><span class="sxs-lookup"><span data-stu-id="69602-112">Binary</span></span>|<span data-ttu-id="69602-113">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="69602-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="69602-114">Цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="69602-114">certFileName</span></span>|<span data-ttu-id="69602-115">String</span><span class="sxs-lookup"><span data-stu-id="69602-115">String</span></span>|<span data-ttu-id="69602-116">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="69602-116">File name to display in UI.</span></span>|
|<span data-ttu-id="69602-117">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="69602-117">certificationAuthority</span></span>|<span data-ttu-id="69602-118">String</span><span class="sxs-lookup"><span data-stu-id="69602-118">String</span></span>|<span data-ttu-id="69602-119">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="69602-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="69602-120">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="69602-120">certificationAuthorityName</span></span>|<span data-ttu-id="69602-121">String</span><span class="sxs-lookup"><span data-stu-id="69602-121">String</span></span>|<span data-ttu-id="69602-122">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="69602-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="69602-123">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="69602-123">certificateTemplateName</span></span>|<span data-ttu-id="69602-124">String</span><span class="sxs-lookup"><span data-stu-id="69602-124">String</span></span>|<span data-ttu-id="69602-125">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="69602-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="69602-126">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="69602-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="69602-127">Int32</span><span class="sxs-lookup"><span data-stu-id="69602-127">Int32</span></span>|<span data-ttu-id="69602-128">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="69602-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="69602-129">Допустимые значения — от 1 до 99</span><span class="sxs-lookup"><span data-stu-id="69602-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="69602-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="69602-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="69602-131">Int32</span><span class="sxs-lookup"><span data-stu-id="69602-131">Int32</span></span>|<span data-ttu-id="69602-132">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="69602-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="69602-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="69602-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="69602-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="69602-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="69602-135">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="69602-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="69602-136">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="69602-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69602-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="69602-137">Relationships</span></span>
<span data-ttu-id="69602-138">Нет</span><span class="sxs-lookup"><span data-stu-id="69602-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69602-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69602-139">JSON Representation</span></span>
<span data-ttu-id="69602-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69602-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```





