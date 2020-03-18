---
title: Тип ресурса Bitlockersystemdrivepolicy.
description: Основные политики шифрования BitLocker.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 313def2a64fdb1a2af57461ba58860361e0de1f2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795731"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="bdbcb-103">Тип ресурса Bitlockersystemdrivepolicy.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="bdbcb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdbcb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdbcb-106">Основные политики шифрования BitLocker.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-106">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="bdbcb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bdbcb-107">Properties</span></span>
|<span data-ttu-id="bdbcb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdbcb-108">Property</span></span>|<span data-ttu-id="bdbcb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bdbcb-109">Type</span></span>|<span data-ttu-id="bdbcb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bdbcb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdbcb-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="bdbcb-111">encryptionMethod</span></span>|[<span data-ttu-id="bdbcb-112">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="bdbcb-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="bdbcb-113">Выберите метод шифрования для дисков операционной системы.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-113">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="bdbcb-114">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="bdbcb-115">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="bdbcb-115">startupAuthenticationRequired</span></span>|<span data-ttu-id="bdbcb-116">Логический</span><span class="sxs-lookup"><span data-stu-id="bdbcb-116">Boolean</span></span>|<span data-ttu-id="bdbcb-117">Требовать дополнительной проверки подлинности при запуске.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-117">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="bdbcb-118">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="bdbcb-118">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="bdbcb-119">Логический</span><span class="sxs-lookup"><span data-stu-id="bdbcb-119">Boolean</span></span>|<span data-ttu-id="bdbcb-120">Указывает, следует ли разрешить BitLocker без совместимого доверенного платформенного модуля (требуется пароль или ключ запуска на USB флэш-накопителе).</span><span class="sxs-lookup"><span data-stu-id="bdbcb-120">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="bdbcb-121">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="bdbcb-121">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="bdbcb-122">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="bdbcb-122">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="bdbcb-123">Указывает, разрешена или не разрешена или необязательная Загрузка TPM.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-123">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="bdbcb-124">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-124">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="bdbcb-125">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="bdbcb-125">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="bdbcb-126">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="bdbcb-126">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="bdbcb-127">Указывает, разрешен ли ПИН-код для запуска TPM, обязательный или запрещенный.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-127">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="bdbcb-128">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-128">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="bdbcb-129">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="bdbcb-129">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="bdbcb-130">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="bdbcb-130">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="bdbcb-131">Указывает, разрешен ли ключ запуска TPM, обязательный, обязательный или запрещенный.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-131">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="bdbcb-132">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-132">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="bdbcb-133">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="bdbcb-133">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="bdbcb-134">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="bdbcb-134">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="bdbcb-135">Указывает, разрешены ли ключ и ключ ПИН-кода для запуска TPM, а какие — обязательные или запрещенные.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-135">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="bdbcb-136">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-136">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="bdbcb-137">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="bdbcb-137">minimumPinLength</span></span>|<span data-ttu-id="bdbcb-138">Int32</span><span class="sxs-lookup"><span data-stu-id="bdbcb-138">Int32</span></span>|<span data-ttu-id="bdbcb-139">Указывает минимальную длину ПИН-кода для запуска.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-139">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="bdbcb-140">Допустимые значения — от 4 до 20.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-140">Valid values 4 to 20</span></span>|
|<span data-ttu-id="bdbcb-141">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="bdbcb-141">recoveryOptions</span></span>|<span data-ttu-id="bdbcb-142">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="bdbcb-142">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="bdbcb-143">Позволяет восстанавливать зашифрованные диски операционной системы BitLocker в отсутствие требуемых сведений о ключе запуска.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-143">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="bdbcb-144">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-144">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="bdbcb-145">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="bdbcb-145">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="bdbcb-146">Логический</span><span class="sxs-lookup"><span data-stu-id="bdbcb-146">Boolean</span></span>|<span data-ttu-id="bdbcb-147">Включение сообщения о восстановлении перед загрузкой и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-147">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="bdbcb-148">Если Рекуирестартупаусентикатион имеет значение false, это значение не влияет.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-148">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="bdbcb-149">пребутрековеримессаже</span><span class="sxs-lookup"><span data-stu-id="bdbcb-149">prebootRecoveryMessage</span></span>|<span data-ttu-id="bdbcb-150">String</span><span class="sxs-lookup"><span data-stu-id="bdbcb-150">String</span></span>|<span data-ttu-id="bdbcb-151">Определяет настраиваемое сообщение о восстановлении.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-151">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="bdbcb-152">пребутрековерюрл</span><span class="sxs-lookup"><span data-stu-id="bdbcb-152">prebootRecoveryUrl</span></span>|<span data-ttu-id="bdbcb-153">String</span><span class="sxs-lookup"><span data-stu-id="bdbcb-153">String</span></span>|<span data-ttu-id="bdbcb-154">Определяет настраиваемый URL-адрес для восстановления.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-154">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdbcb-155">Связи</span><span class="sxs-lookup"><span data-stu-id="bdbcb-155">Relationships</span></span>
<span data-ttu-id="bdbcb-156">Нет</span><span class="sxs-lookup"><span data-stu-id="bdbcb-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdbcb-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bdbcb-157">JSON Representation</span></span>
<span data-ttu-id="bdbcb-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdbcb-158">Here is a JSON representation of the resource.</span></span>
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



