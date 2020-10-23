---
title: тип перечисления Филеваултстате
description: Состояние Филеваулт
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c1ef23c9428b2d8b5ed82c5264d829eb0b1febde
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734037"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="ff268-103">тип перечисления Филеваултстате</span><span class="sxs-lookup"><span data-stu-id="ff268-103">fileVaultState enum type</span></span>

<span data-ttu-id="ff268-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff268-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff268-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff268-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff268-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff268-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff268-107">Состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="ff268-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="ff268-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ff268-108">Members</span></span>
|<span data-ttu-id="ff268-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ff268-109">Member</span></span>|<span data-ttu-id="ff268-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ff268-110">Value</span></span>|<span data-ttu-id="ff268-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ff268-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff268-112">success</span><span class="sxs-lookup"><span data-stu-id="ff268-112">success</span></span>|<span data-ttu-id="ff268-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ff268-113">0</span></span>|<span data-ttu-id="ff268-114">Успешное состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="ff268-114">FileVault State Success</span></span>|
|<span data-ttu-id="ff268-115">дривинкриптедбюсер</span><span class="sxs-lookup"><span data-stu-id="ff268-115">driveEncryptedByUser</span></span>|<span data-ttu-id="ff268-116">1,1</span><span class="sxs-lookup"><span data-stu-id="ff268-116">1</span></span>|<span data-ttu-id="ff268-117">Филеваулт был включен пользователем и не управляется политикой</span><span class="sxs-lookup"><span data-stu-id="ff268-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="ff268-118">усердеферреденкриптион</span><span class="sxs-lookup"><span data-stu-id="ff268-118">userDeferredEncryption</span></span>|<span data-ttu-id="ff268-119">2</span><span class="sxs-lookup"><span data-stu-id="ff268-119">2</span></span>|<span data-ttu-id="ff268-120">Политика Филеваулт успешно установлена, но пользователь не начал шифрование</span><span class="sxs-lookup"><span data-stu-id="ff268-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="ff268-121">ескровнотенаблед</span><span class="sxs-lookup"><span data-stu-id="ff268-121">escrowNotEnabled</span></span>|<span data-ttu-id="ff268-122">4 </span><span class="sxs-lookup"><span data-stu-id="ff268-122">4</span></span>|<span data-ttu-id="ff268-123">Филеваулт не включен параметр "депонирование ключей восстановления"</span><span class="sxs-lookup"><span data-stu-id="ff268-123">FileVault recovery key escrow is not enabled</span></span>|





