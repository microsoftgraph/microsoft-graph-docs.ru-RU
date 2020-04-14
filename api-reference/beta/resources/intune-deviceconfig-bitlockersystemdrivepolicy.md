---
title: Тип ресурса Bitlockersystemdrivepolicy.
description: Основные политики шифрования BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82ed6d717c58f740dd25d2aff18478ced48c4641
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453675"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="a4ac2-103">Тип ресурса Bitlockersystemdrivepolicy.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-103">bitLockerSystemDrivePolicy resource type</span></span>

<span data-ttu-id="a4ac2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4ac2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4ac2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4ac2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4ac2-107">Основные политики шифрования BitLocker.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="a4ac2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4ac2-108">Properties</span></span>
|<span data-ttu-id="a4ac2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4ac2-109">Property</span></span>|<span data-ttu-id="a4ac2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a4ac2-110">Type</span></span>|<span data-ttu-id="a4ac2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ac2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4ac2-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a4ac2-112">encryptionMethod</span></span>|[<span data-ttu-id="a4ac2-113">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="a4ac2-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="a4ac2-114">Выберите метод шифрования для дисков операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="a4ac2-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="a4ac2-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="a4ac2-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="a4ac2-117">Логическое</span><span class="sxs-lookup"><span data-stu-id="a4ac2-117">Boolean</span></span>|<span data-ttu-id="a4ac2-118">Требовать дополнительной проверки подлинности при запуске.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="a4ac2-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="a4ac2-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="a4ac2-120">Логическое</span><span class="sxs-lookup"><span data-stu-id="a4ac2-120">Boolean</span></span>|<span data-ttu-id="a4ac2-121">Указывает, следует ли разрешить BitLocker без совместимого доверенного платформенного модуля (требуется пароль или ключ запуска на USB флэш-накопителе).</span><span class="sxs-lookup"><span data-stu-id="a4ac2-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="a4ac2-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="a4ac2-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="a4ac2-123">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="a4ac2-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a4ac2-124">Указывает, разрешена или не разрешена или необязательная Загрузка TPM.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="a4ac2-125">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a4ac2-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="a4ac2-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="a4ac2-127">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="a4ac2-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a4ac2-128">Указывает, разрешен ли ПИН-код для запуска TPM, обязательный или запрещенный.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="a4ac2-129">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a4ac2-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="a4ac2-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="a4ac2-131">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="a4ac2-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a4ac2-132">Указывает, разрешен ли ключ запуска TPM, обязательный, обязательный или запрещенный.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="a4ac2-133">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a4ac2-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="a4ac2-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="a4ac2-135">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="a4ac2-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a4ac2-136">Указывает, разрешены ли ключ и ключ ПИН-кода для запуска TPM, а какие — обязательные или запрещенные.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="a4ac2-137">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="a4ac2-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="a4ac2-138">minimumPinLength</span></span>|<span data-ttu-id="a4ac2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a4ac2-139">Int32</span></span>|<span data-ttu-id="a4ac2-140">Указывает минимальную длину ПИН-кода для запуска.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="a4ac2-141">Допустимые значения — от 4 до 20.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="a4ac2-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="a4ac2-142">recoveryOptions</span></span>|<span data-ttu-id="a4ac2-143">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="a4ac2-143">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="a4ac2-144">Позволяет восстанавливать зашифрованные диски операционной системы BitLocker в отсутствие требуемых сведений о ключе запуска.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="a4ac2-145">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="a4ac2-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="a4ac2-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="a4ac2-147">Логическое</span><span class="sxs-lookup"><span data-stu-id="a4ac2-147">Boolean</span></span>|<span data-ttu-id="a4ac2-148">Включение сообщения о восстановлении перед загрузкой и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="a4ac2-149">Если Рекуирестартупаусентикатион имеет значение false, это значение не влияет.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="a4ac2-150">пребутрековеримессаже</span><span class="sxs-lookup"><span data-stu-id="a4ac2-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="a4ac2-151">String</span><span class="sxs-lookup"><span data-stu-id="a4ac2-151">String</span></span>|<span data-ttu-id="a4ac2-152">Определяет настраиваемое сообщение о восстановлении.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="a4ac2-153">пребутрековерюрл</span><span class="sxs-lookup"><span data-stu-id="a4ac2-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="a4ac2-154">String</span><span class="sxs-lookup"><span data-stu-id="a4ac2-154">String</span></span>|<span data-ttu-id="a4ac2-155">Определяет настраиваемый URL-адрес для восстановления.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4ac2-156">Связи</span><span class="sxs-lookup"><span data-stu-id="a4ac2-156">Relationships</span></span>
<span data-ttu-id="a4ac2-157">Нет</span><span class="sxs-lookup"><span data-stu-id="a4ac2-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4ac2-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4ac2-158">JSON Representation</span></span>
<span data-ttu-id="a4ac2-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4ac2-159">Here is a JSON representation of the resource.</span></span>
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



