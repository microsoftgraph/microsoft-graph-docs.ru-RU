---
title: тип перечисления Филеваултстате
description: Состояние Филеваулт
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2d7f69413ac7fd4be1e857951b2a70aac0fe7bc3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444318"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="d8bd4-103">тип перечисления Филеваултстате</span><span class="sxs-lookup"><span data-stu-id="d8bd4-103">fileVaultState enum type</span></span>

<span data-ttu-id="d8bd4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8bd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8bd4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8bd4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8bd4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8bd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8bd4-107">Состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="d8bd4-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="d8bd4-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d8bd4-108">Members</span></span>
|<span data-ttu-id="d8bd4-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d8bd4-109">Member</span></span>|<span data-ttu-id="d8bd4-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d8bd4-110">Value</span></span>|<span data-ttu-id="d8bd4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8bd4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8bd4-112">success</span><span class="sxs-lookup"><span data-stu-id="d8bd4-112">success</span></span>|<span data-ttu-id="d8bd4-113">нуль</span><span class="sxs-lookup"><span data-stu-id="d8bd4-113">0</span></span>|<span data-ttu-id="d8bd4-114">Успешное состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="d8bd4-114">FileVault State Success</span></span>|
|<span data-ttu-id="d8bd4-115">дривинкриптедбюсер</span><span class="sxs-lookup"><span data-stu-id="d8bd4-115">driveEncryptedByUser</span></span>|<span data-ttu-id="d8bd4-116">1,1</span><span class="sxs-lookup"><span data-stu-id="d8bd4-116">1</span></span>|<span data-ttu-id="d8bd4-117">Филеваулт был включен пользователем и не управляется политикой</span><span class="sxs-lookup"><span data-stu-id="d8bd4-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="d8bd4-118">усердеферреденкриптион</span><span class="sxs-lookup"><span data-stu-id="d8bd4-118">userDeferredEncryption</span></span>|<span data-ttu-id="d8bd4-119">2</span><span class="sxs-lookup"><span data-stu-id="d8bd4-119">2</span></span>|<span data-ttu-id="d8bd4-120">Политика Филеваулт успешно установлена, но пользователь не начал шифрование</span><span class="sxs-lookup"><span data-stu-id="d8bd4-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="d8bd4-121">ескровнотенаблед</span><span class="sxs-lookup"><span data-stu-id="d8bd4-121">escrowNotEnabled</span></span>|<span data-ttu-id="d8bd4-122">4 </span><span class="sxs-lookup"><span data-stu-id="d8bd4-122">4</span></span>|<span data-ttu-id="d8bd4-123">Филеваулт не включен параметр "депонирование ключей восстановления"</span><span class="sxs-lookup"><span data-stu-id="d8bd4-123">FileVault recovery key escrow is not enabled</span></span>|



