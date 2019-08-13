---
title: тип перечисления Филеваултстате
description: Состояние Филеваулт
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 54e8076dc4b4f6ab20f7790d2a650de6c07aa702
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325570"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="5d575-103">тип перечисления Филеваултстате</span><span class="sxs-lookup"><span data-stu-id="5d575-103">fileVaultState enum type</span></span>

> <span data-ttu-id="5d575-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d575-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d575-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d575-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d575-106">Состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="5d575-106">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="5d575-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5d575-107">Members</span></span>
|<span data-ttu-id="5d575-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5d575-108">Member</span></span>|<span data-ttu-id="5d575-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5d575-109">Value</span></span>|<span data-ttu-id="5d575-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5d575-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d575-111">success</span><span class="sxs-lookup"><span data-stu-id="5d575-111">success</span></span>|<span data-ttu-id="5d575-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5d575-112">0</span></span>|<span data-ttu-id="5d575-113">Успешное состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="5d575-113">FileVault State Success</span></span>|
|<span data-ttu-id="5d575-114">дривинкриптедбюсер</span><span class="sxs-lookup"><span data-stu-id="5d575-114">driveEncryptedByUser</span></span>|<span data-ttu-id="5d575-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5d575-115">1</span></span>|<span data-ttu-id="5d575-116">Филеваулт был включен пользователем и не управляется политикой</span><span class="sxs-lookup"><span data-stu-id="5d575-116">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="5d575-117">усердеферреденкриптион</span><span class="sxs-lookup"><span data-stu-id="5d575-117">userDeferredEncryption</span></span>|<span data-ttu-id="5d575-118">2</span><span class="sxs-lookup"><span data-stu-id="5d575-118">2</span></span>|<span data-ttu-id="5d575-119">Политика Филеваулт успешно установлена, но пользователь не начал шифрование</span><span class="sxs-lookup"><span data-stu-id="5d575-119">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="5d575-120">ескровнотенаблед</span><span class="sxs-lookup"><span data-stu-id="5d575-120">escrowNotEnabled</span></span>|<span data-ttu-id="5d575-121">SP4</span><span class="sxs-lookup"><span data-stu-id="5d575-121">4</span></span>|<span data-ttu-id="5d575-122">Филеваулт не включен параметр "депонирование ключей восстановления"</span><span class="sxs-lookup"><span data-stu-id="5d575-122">FileVault recovery key escrow is not enabled</span></span>|



