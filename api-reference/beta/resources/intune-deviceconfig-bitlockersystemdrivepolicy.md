---
title: Тип ресурса bitLockerSystemDrivePolicy
description: Базовый политики шифрования BitLocker.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b63d075538508941d012df1e44f7cb563fed20d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425710"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="d588c-103">Тип ресурса bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d588c-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="d588c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d588c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d588c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d588c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d588c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d588c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d588c-107">Базовый политики шифрования BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d588c-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="d588c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d588c-108">Properties</span></span>
|<span data-ttu-id="d588c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d588c-109">Property</span></span>|<span data-ttu-id="d588c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d588c-110">Type</span></span>|<span data-ttu-id="d588c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d588c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d588c-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d588c-112">encryptionMethod</span></span>|[<span data-ttu-id="d588c-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d588c-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="d588c-114">Выберите метод шифрования для дисков операционной системы.</span><span class="sxs-lookup"><span data-stu-id="d588c-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="d588c-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="d588c-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="d588c-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="d588c-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="d588c-117">Логический</span><span class="sxs-lookup"><span data-stu-id="d588c-117">Boolean</span></span>|<span data-ttu-id="d588c-118">Требовать дополнительную проверку подлинности при запуске системы.</span><span class="sxs-lookup"><span data-stu-id="d588c-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="d588c-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="d588c-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="d588c-120">Логический</span><span class="sxs-lookup"><span data-stu-id="d588c-120">Boolean</span></span>|<span data-ttu-id="d588c-121">Указывает, следует ли разрешить BitLocker без совместимого TPM (требуется пароль или ключ запуска на флэш-накопитель USB).</span><span class="sxs-lookup"><span data-stu-id="d588c-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="d588c-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="d588c-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="d588c-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="d588c-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d588c-124">Указывает, является ли запуска TPM разрешенных/необходимые/не разрешены.</span><span class="sxs-lookup"><span data-stu-id="d588c-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="d588c-125">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d588c-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d588c-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="d588c-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="d588c-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="d588c-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d588c-128">Указывает, является ли ПИН-кода запуска TPM разрешенных/необходимые/не разрешены.</span><span class="sxs-lookup"><span data-stu-id="d588c-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="d588c-129">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d588c-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d588c-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="d588c-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="d588c-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="d588c-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d588c-132">Указывает, является ли ключ запуска TPM разрешенных/необходимые/не разрешены.</span><span class="sxs-lookup"><span data-stu-id="d588c-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="d588c-133">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d588c-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d588c-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="d588c-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="d588c-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="d588c-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d588c-136">Указывает, если прикрепление запуска TPM и ключ разрешенных/необходимые/не разрешены.</span><span class="sxs-lookup"><span data-stu-id="d588c-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="d588c-137">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d588c-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d588c-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="d588c-138">minimumPinLength</span></span>|<span data-ttu-id="d588c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d588c-139">Int32</span></span>|<span data-ttu-id="d588c-140">Указывает минимальную длину ПИН-кодов запуска.</span><span class="sxs-lookup"><span data-stu-id="d588c-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="d588c-141">Допустимые значения 4 до 20</span><span class="sxs-lookup"><span data-stu-id="d588c-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="d588c-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="d588c-142">recoveryOptions</span></span>|<span data-ttu-id="d588c-143">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="d588c-143">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="d588c-144">Разрешает Восстановление зашифрованного BitLocker дисков операционной системы в случае отсутствия данные ключа требуется запуска.</span><span class="sxs-lookup"><span data-stu-id="d588c-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="d588c-145">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d588c-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="d588c-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="d588c-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="d588c-147">Логический</span><span class="sxs-lookup"><span data-stu-id="d588c-147">Boolean</span></span>|<span data-ttu-id="d588c-148">Включение восстановления до загрузки сообщение и URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="d588c-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="d588c-149">Если requireStartupAuthentication имеет значение false, это значение не влияет на.</span><span class="sxs-lookup"><span data-stu-id="d588c-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="d588c-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="d588c-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="d588c-151">String</span><span class="sxs-lookup"><span data-stu-id="d588c-151">String</span></span>|<span data-ttu-id="d588c-152">Определяет сообщение настраиваемого восстановления.</span><span class="sxs-lookup"><span data-stu-id="d588c-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="d588c-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="d588c-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="d588c-154">String</span><span class="sxs-lookup"><span data-stu-id="d588c-154">String</span></span>|<span data-ttu-id="d588c-155">Определяет URL-адрес настраиваемого восстановления.</span><span class="sxs-lookup"><span data-stu-id="d588c-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d588c-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="d588c-156">Relationships</span></span>
<span data-ttu-id="d588c-157">Нет</span><span class="sxs-lookup"><span data-stu-id="d588c-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d588c-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d588c-158">JSON Representation</span></span>
<span data-ttu-id="d588c-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d588c-159">Here is a JSON representation of the resource.</span></span>
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




