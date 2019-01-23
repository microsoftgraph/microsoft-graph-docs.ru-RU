---
title: Тип ресурса iosEduCertificateSettings
description: Доверенные корневые папки и PFX сертификаты для iOS EDU.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d23b379dea7a75e4ae79029845cd6e9f956503c0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423554"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="09320-103">Тип ресурса iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="09320-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="09320-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="09320-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="09320-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09320-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09320-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09320-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09320-107">Доверенные корневые папки и PFX сертификаты для iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="09320-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="09320-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="09320-108">Properties</span></span>
|<span data-ttu-id="09320-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="09320-109">Property</span></span>|<span data-ttu-id="09320-110">Тип</span><span class="sxs-lookup"><span data-stu-id="09320-110">Type</span></span>|<span data-ttu-id="09320-111">Описание</span><span class="sxs-lookup"><span data-stu-id="09320-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09320-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="09320-112">trustedRootCertificate</span></span>|<span data-ttu-id="09320-113">Binary</span><span class="sxs-lookup"><span data-stu-id="09320-113">Binary</span></span>|<span data-ttu-id="09320-114">Доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="09320-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="09320-115">certFileName</span><span class="sxs-lookup"><span data-stu-id="09320-115">certFileName</span></span>|<span data-ttu-id="09320-116">String</span><span class="sxs-lookup"><span data-stu-id="09320-116">String</span></span>|<span data-ttu-id="09320-117">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="09320-117">File name to display in UI.</span></span>|
|<span data-ttu-id="09320-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="09320-118">certificationAuthority</span></span>|<span data-ttu-id="09320-119">String</span><span class="sxs-lookup"><span data-stu-id="09320-119">String</span></span>|<span data-ttu-id="09320-120">PKCS центром сертификации.</span><span class="sxs-lookup"><span data-stu-id="09320-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="09320-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="09320-121">certificationAuthorityName</span></span>|<span data-ttu-id="09320-122">String</span><span class="sxs-lookup"><span data-stu-id="09320-122">String</span></span>|<span data-ttu-id="09320-123">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="09320-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="09320-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="09320-124">certificateTemplateName</span></span>|<span data-ttu-id="09320-125">String</span><span class="sxs-lookup"><span data-stu-id="09320-125">String</span></span>|<span data-ttu-id="09320-126">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="09320-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="09320-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="09320-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="09320-128">Int32</span><span class="sxs-lookup"><span data-stu-id="09320-128">Int32</span></span>|<span data-ttu-id="09320-129">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="09320-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="09320-130">Допустимые значения от 1 до 99</span><span class="sxs-lookup"><span data-stu-id="09320-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="09320-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="09320-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="09320-132">Int32</span><span class="sxs-lookup"><span data-stu-id="09320-132">Int32</span></span>|<span data-ttu-id="09320-133">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="09320-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="09320-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="09320-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="09320-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="09320-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="09320-136">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="09320-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="09320-137">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="09320-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09320-138">Связи</span><span class="sxs-lookup"><span data-stu-id="09320-138">Relationships</span></span>
<span data-ttu-id="09320-139">Нет</span><span class="sxs-lookup"><span data-stu-id="09320-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09320-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09320-140">JSON Representation</span></span>
<span data-ttu-id="09320-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09320-141">Here is a JSON representation of the resource.</span></span>
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




