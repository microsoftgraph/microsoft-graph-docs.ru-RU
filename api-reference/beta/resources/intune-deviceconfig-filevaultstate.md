---
title: тип перечисления Филеваултстате
description: Состояние Филеваулт
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a9aa7c0b11a155597911f64882f5b6d424a2b129
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294524"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="38f6a-103">тип перечисления Филеваултстате</span><span class="sxs-lookup"><span data-stu-id="38f6a-103">fileVaultState enum type</span></span>

<span data-ttu-id="38f6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38f6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38f6a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38f6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38f6a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38f6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38f6a-107">Состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="38f6a-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="38f6a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="38f6a-108">Members</span></span>
|<span data-ttu-id="38f6a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="38f6a-109">Member</span></span>|<span data-ttu-id="38f6a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="38f6a-110">Value</span></span>|<span data-ttu-id="38f6a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38f6a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38f6a-112">success</span><span class="sxs-lookup"><span data-stu-id="38f6a-112">success</span></span>|<span data-ttu-id="38f6a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="38f6a-113">0</span></span>|<span data-ttu-id="38f6a-114">Успешное состояние Филеваулт</span><span class="sxs-lookup"><span data-stu-id="38f6a-114">FileVault State Success</span></span>|
|<span data-ttu-id="38f6a-115">дривинкриптедбюсер</span><span class="sxs-lookup"><span data-stu-id="38f6a-115">driveEncryptedByUser</span></span>|<span data-ttu-id="38f6a-116">1,1</span><span class="sxs-lookup"><span data-stu-id="38f6a-116">1</span></span>|<span data-ttu-id="38f6a-117">Филеваулт был включен пользователем и не управляется политикой</span><span class="sxs-lookup"><span data-stu-id="38f6a-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="38f6a-118">усердеферреденкриптион</span><span class="sxs-lookup"><span data-stu-id="38f6a-118">userDeferredEncryption</span></span>|<span data-ttu-id="38f6a-119">2</span><span class="sxs-lookup"><span data-stu-id="38f6a-119">2</span></span>|<span data-ttu-id="38f6a-120">Политика Филеваулт успешно установлена, но пользователь не начал шифрование</span><span class="sxs-lookup"><span data-stu-id="38f6a-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="38f6a-121">ескровнотенаблед</span><span class="sxs-lookup"><span data-stu-id="38f6a-121">escrowNotEnabled</span></span>|<span data-ttu-id="38f6a-122">4 </span><span class="sxs-lookup"><span data-stu-id="38f6a-122">4</span></span>|<span data-ttu-id="38f6a-123">Филеваулт не включен параметр "депонирование ключей восстановления"</span><span class="sxs-lookup"><span data-stu-id="38f6a-123">FileVault recovery key escrow is not enabled</span></span>|




