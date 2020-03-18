---
title: тип перечисления Филеваултстате
description: Состояние Филеваулт
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1efe284a4d6bad3685c6fbf9c4003153a3aca913
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791767"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="714b9-103">тип перечисления Филеваултстате</span><span class="sxs-lookup"><span data-stu-id="714b9-103">fileVaultState enum type</span></span>

> <span data-ttu-id="714b9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="714b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="714b9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="714b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="714b9-106">Состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="714b9-106">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="714b9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="714b9-107">Members</span></span>
|<span data-ttu-id="714b9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="714b9-108">Member</span></span>|<span data-ttu-id="714b9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="714b9-109">Value</span></span>|<span data-ttu-id="714b9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="714b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="714b9-111">success</span><span class="sxs-lookup"><span data-stu-id="714b9-111">success</span></span>|<span data-ttu-id="714b9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="714b9-112">0</span></span>|<span data-ttu-id="714b9-113">Успешное состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="714b9-113">FileVault State Success</span></span>|
|<span data-ttu-id="714b9-114">дривинкриптедбюсер</span><span class="sxs-lookup"><span data-stu-id="714b9-114">driveEncryptedByUser</span></span>|<span data-ttu-id="714b9-115">1,1</span><span class="sxs-lookup"><span data-stu-id="714b9-115">1</span></span>|<span data-ttu-id="714b9-116">Филеваулт был включен пользователем и не управляется политикой</span><span class="sxs-lookup"><span data-stu-id="714b9-116">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="714b9-117">усердеферреденкриптион</span><span class="sxs-lookup"><span data-stu-id="714b9-117">userDeferredEncryption</span></span>|<span data-ttu-id="714b9-118">2</span><span class="sxs-lookup"><span data-stu-id="714b9-118">2</span></span>|<span data-ttu-id="714b9-119">Политика Филеваулт успешно установлена, но пользователь не начал шифрование</span><span class="sxs-lookup"><span data-stu-id="714b9-119">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="714b9-120">ескровнотенаблед</span><span class="sxs-lookup"><span data-stu-id="714b9-120">escrowNotEnabled</span></span>|<span data-ttu-id="714b9-121">4 </span><span class="sxs-lookup"><span data-stu-id="714b9-121">4</span></span>|<span data-ttu-id="714b9-122">Филеваулт не включен параметр "депонирование ключей восстановления"</span><span class="sxs-lookup"><span data-stu-id="714b9-122">FileVault recovery key escrow is not enabled</span></span>|



