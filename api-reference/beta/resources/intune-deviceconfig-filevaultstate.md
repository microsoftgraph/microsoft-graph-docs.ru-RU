---
title: тип перечисления Филеваултстате
description: Состояние Филеваулт
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8f2fa72d2db91ba000209332aec3d59579cba822
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530001"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="a3853-103">тип перечисления Филеваултстате</span><span class="sxs-lookup"><span data-stu-id="a3853-103">fileVaultState enum type</span></span>

<span data-ttu-id="a3853-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3853-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3853-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3853-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3853-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3853-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3853-107">Состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="a3853-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="a3853-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a3853-108">Members</span></span>
|<span data-ttu-id="a3853-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a3853-109">Member</span></span>|<span data-ttu-id="a3853-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a3853-110">Value</span></span>|<span data-ttu-id="a3853-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a3853-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3853-112">success</span><span class="sxs-lookup"><span data-stu-id="a3853-112">success</span></span>|<span data-ttu-id="a3853-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a3853-113">0</span></span>|<span data-ttu-id="a3853-114">Успешное состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="a3853-114">FileVault State Success</span></span>|
|<span data-ttu-id="a3853-115">дривинкриптедбюсер</span><span class="sxs-lookup"><span data-stu-id="a3853-115">driveEncryptedByUser</span></span>|<span data-ttu-id="a3853-116">1 </span><span class="sxs-lookup"><span data-stu-id="a3853-116">1</span></span>|<span data-ttu-id="a3853-117">Филеваулт был включен пользователем и не управляется политикой</span><span class="sxs-lookup"><span data-stu-id="a3853-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="a3853-118">усердеферреденкриптион</span><span class="sxs-lookup"><span data-stu-id="a3853-118">userDeferredEncryption</span></span>|<span data-ttu-id="a3853-119">2 </span><span class="sxs-lookup"><span data-stu-id="a3853-119">2</span></span>|<span data-ttu-id="a3853-120">Политика Филеваулт успешно установлена, но пользователь не начал шифрование</span><span class="sxs-lookup"><span data-stu-id="a3853-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="a3853-121">ескровнотенаблед</span><span class="sxs-lookup"><span data-stu-id="a3853-121">escrowNotEnabled</span></span>|<span data-ttu-id="a3853-122">4 </span><span class="sxs-lookup"><span data-stu-id="a3853-122">4</span></span>|<span data-ttu-id="a3853-123">Филеваулт не включен параметр "депонирование ключей восстановления"</span><span class="sxs-lookup"><span data-stu-id="a3853-123">FileVault recovery key escrow is not enabled</span></span>|



