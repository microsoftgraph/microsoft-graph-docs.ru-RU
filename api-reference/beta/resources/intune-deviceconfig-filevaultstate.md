---
title: тип перечисления Филеваултстате
description: Состояние Филеваулт
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f122d62f85f90825f5fe3129ec2a314d5886e6f2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726179"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="c5943-103">тип перечисления Филеваултстате</span><span class="sxs-lookup"><span data-stu-id="c5943-103">fileVaultState enum type</span></span>

> <span data-ttu-id="c5943-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5943-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5943-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5943-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5943-106">Состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="c5943-106">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="c5943-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c5943-107">Members</span></span>
|<span data-ttu-id="c5943-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c5943-108">Member</span></span>|<span data-ttu-id="c5943-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c5943-109">Value</span></span>|<span data-ttu-id="c5943-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5943-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5943-111">success</span><span class="sxs-lookup"><span data-stu-id="c5943-111">success</span></span>|<span data-ttu-id="c5943-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c5943-112">0</span></span>|<span data-ttu-id="c5943-113">Успешное состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="c5943-113">FileVault State Success</span></span>|
|<span data-ttu-id="c5943-114">Дривинкриптедбюсер</span><span class="sxs-lookup"><span data-stu-id="c5943-114">driveEncryptedByUser</span></span>|<span data-ttu-id="c5943-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c5943-115">1</span></span>|<span data-ttu-id="c5943-116">Филеваулт был включен пользователем и не управляется политикой</span><span class="sxs-lookup"><span data-stu-id="c5943-116">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="c5943-117">Усердеферреденкриптион</span><span class="sxs-lookup"><span data-stu-id="c5943-117">userDeferredEncryption</span></span>|<span data-ttu-id="c5943-118">2</span><span class="sxs-lookup"><span data-stu-id="c5943-118">2</span></span>|<span data-ttu-id="c5943-119">Политика Филеваулт успешно установлена, но пользователь не начал шифрование</span><span class="sxs-lookup"><span data-stu-id="c5943-119">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="c5943-120">Ескровнотенаблед</span><span class="sxs-lookup"><span data-stu-id="c5943-120">escrowNotEnabled</span></span>|<span data-ttu-id="c5943-121">SP4</span><span class="sxs-lookup"><span data-stu-id="c5943-121">4</span></span>|<span data-ttu-id="c5943-122">Филеваулт не включен параметр "депонирование ключей восстановления"</span><span class="sxs-lookup"><span data-stu-id="c5943-122">FileVault recovery key escrow is not enabled</span></span>|







