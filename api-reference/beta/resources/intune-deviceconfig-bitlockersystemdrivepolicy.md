---
title: Тип ресурса Bitlockersystemdrivepolicy.
description: Основные политики шифрования BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2ef33abdcb8cc5c27fe1e0cd6146f0f736202aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040023"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="01748-103">Тип ресурса Bitlockersystemdrivepolicy.</span><span class="sxs-lookup"><span data-stu-id="01748-103">bitLockerSystemDrivePolicy resource type</span></span>

<span data-ttu-id="01748-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01748-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01748-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01748-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01748-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01748-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01748-107">Основные политики шифрования BitLocker.</span><span class="sxs-lookup"><span data-stu-id="01748-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="01748-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="01748-108">Properties</span></span>
|<span data-ttu-id="01748-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="01748-109">Property</span></span>|<span data-ttu-id="01748-110">Тип</span><span class="sxs-lookup"><span data-stu-id="01748-110">Type</span></span>|<span data-ttu-id="01748-111">Описание</span><span class="sxs-lookup"><span data-stu-id="01748-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01748-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="01748-112">encryptionMethod</span></span>|[<span data-ttu-id="01748-113">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="01748-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="01748-114">Выберите метод шифрования для дисков операционной системы.</span><span class="sxs-lookup"><span data-stu-id="01748-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="01748-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="01748-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="01748-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="01748-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="01748-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="01748-117">Boolean</span></span>|<span data-ttu-id="01748-118">Требовать дополнительной проверки подлинности при запуске.</span><span class="sxs-lookup"><span data-stu-id="01748-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="01748-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="01748-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="01748-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="01748-120">Boolean</span></span>|<span data-ttu-id="01748-121">Указывает, следует ли разрешить BitLocker без совместимого доверенного платформенного модуля (требуется пароль или ключ запуска на USB флэш-накопителе).</span><span class="sxs-lookup"><span data-stu-id="01748-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="01748-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="01748-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="01748-123">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="01748-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="01748-124">Указывает, разрешена или не разрешена или необязательная Загрузка TPM.</span><span class="sxs-lookup"><span data-stu-id="01748-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="01748-125">Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="01748-125">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="01748-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="01748-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="01748-127">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="01748-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="01748-128">Указывает, разрешен ли ПИН-код для запуска TPM, обязательный или запрещенный.</span><span class="sxs-lookup"><span data-stu-id="01748-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="01748-129">Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="01748-129">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="01748-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="01748-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="01748-131">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="01748-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="01748-132">Указывает, разрешен ли ключ запуска TPM, обязательный, обязательный или запрещенный.</span><span class="sxs-lookup"><span data-stu-id="01748-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="01748-133">Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="01748-133">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="01748-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="01748-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="01748-135">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="01748-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="01748-136">Указывает, разрешены ли ключ и ключ ПИН-кода для запуска TPM, а какие — обязательные или запрещенные.</span><span class="sxs-lookup"><span data-stu-id="01748-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="01748-137">Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="01748-137">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="01748-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="01748-138">minimumPinLength</span></span>|<span data-ttu-id="01748-139">Int32</span><span class="sxs-lookup"><span data-stu-id="01748-139">Int32</span></span>|<span data-ttu-id="01748-140">Указывает минимальную длину ПИН-кода для запуска.</span><span class="sxs-lookup"><span data-stu-id="01748-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="01748-141">Допустимые значения — от 4 до 20.</span><span class="sxs-lookup"><span data-stu-id="01748-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="01748-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="01748-142">recoveryOptions</span></span>|<span data-ttu-id="01748-143">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="01748-143">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="01748-144">Позволяет восстанавливать зашифрованные диски операционной системы BitLocker в отсутствие требуемых сведений о ключе запуска.</span><span class="sxs-lookup"><span data-stu-id="01748-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="01748-145">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="01748-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="01748-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="01748-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="01748-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="01748-147">Boolean</span></span>|<span data-ttu-id="01748-148">Включение сообщения о восстановлении перед загрузкой и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="01748-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="01748-149">Если Рекуирестартупаусентикатион имеет значение false, это значение не влияет.</span><span class="sxs-lookup"><span data-stu-id="01748-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="01748-150">пребутрековеримессаже</span><span class="sxs-lookup"><span data-stu-id="01748-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="01748-151">String</span><span class="sxs-lookup"><span data-stu-id="01748-151">String</span></span>|<span data-ttu-id="01748-152">Определяет настраиваемое сообщение о восстановлении.</span><span class="sxs-lookup"><span data-stu-id="01748-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="01748-153">пребутрековерюрл</span><span class="sxs-lookup"><span data-stu-id="01748-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="01748-154">String</span><span class="sxs-lookup"><span data-stu-id="01748-154">String</span></span>|<span data-ttu-id="01748-155">Определяет настраиваемый URL-адрес для восстановления.</span><span class="sxs-lookup"><span data-stu-id="01748-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01748-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="01748-156">Relationships</span></span>
<span data-ttu-id="01748-157">Нет</span><span class="sxs-lookup"><span data-stu-id="01748-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01748-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01748-158">JSON Representation</span></span>
<span data-ttu-id="01748-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01748-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```






