---
title: Тип ресурса Иоседуцертификатесеттингс
description: Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f772ee8f484b2b8bc42a6ed48298dc5a17016afc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791620"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="f5349-103">Тип ресурса Иоседуцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="f5349-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="f5349-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5349-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5349-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5349-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5349-106">Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="f5349-106">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="f5349-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5349-107">Properties</span></span>
|<span data-ttu-id="f5349-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5349-108">Property</span></span>|<span data-ttu-id="f5349-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f5349-109">Type</span></span>|<span data-ttu-id="f5349-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f5349-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5349-111">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="f5349-111">trustedRootCertificate</span></span>|<span data-ttu-id="f5349-112">Binary</span><span class="sxs-lookup"><span data-stu-id="f5349-112">Binary</span></span>|<span data-ttu-id="f5349-113">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="f5349-113">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="f5349-114">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="f5349-114">certFileName</span></span>|<span data-ttu-id="f5349-115">String</span><span class="sxs-lookup"><span data-stu-id="f5349-115">String</span></span>|<span data-ttu-id="f5349-116">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="f5349-116">File name to display in UI.</span></span>|
|<span data-ttu-id="f5349-117">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="f5349-117">certificationAuthority</span></span>|<span data-ttu-id="f5349-118">String</span><span class="sxs-lookup"><span data-stu-id="f5349-118">String</span></span>|<span data-ttu-id="f5349-119">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="f5349-119">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="f5349-120">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="f5349-120">certificationAuthorityName</span></span>|<span data-ttu-id="f5349-121">String</span><span class="sxs-lookup"><span data-stu-id="f5349-121">String</span></span>|<span data-ttu-id="f5349-122">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="f5349-122">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="f5349-123">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="f5349-123">certificateTemplateName</span></span>|<span data-ttu-id="f5349-124">String</span><span class="sxs-lookup"><span data-stu-id="f5349-124">String</span></span>|<span data-ttu-id="f5349-125">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="f5349-125">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="f5349-126">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="f5349-126">renewalThresholdPercentage</span></span>|<span data-ttu-id="f5349-127">Int32</span><span class="sxs-lookup"><span data-stu-id="f5349-127">Int32</span></span>|<span data-ttu-id="f5349-128">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="f5349-128">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f5349-129">Допустимые значения — от 1 до 99</span><span class="sxs-lookup"><span data-stu-id="f5349-129">Valid values 1 to 99</span></span>|
|<span data-ttu-id="f5349-130">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f5349-130">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f5349-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f5349-131">Int32</span></span>|<span data-ttu-id="f5349-132">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f5349-132">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="f5349-133">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f5349-133">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f5349-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f5349-134">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f5349-135">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f5349-135">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f5349-136">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f5349-136">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5349-137">Связи</span><span class="sxs-lookup"><span data-stu-id="f5349-137">Relationships</span></span>
<span data-ttu-id="f5349-138">Нет</span><span class="sxs-lookup"><span data-stu-id="f5349-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5349-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5349-139">JSON Representation</span></span>
<span data-ttu-id="f5349-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5349-140">Here is a JSON representation of the resource.</span></span>
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



