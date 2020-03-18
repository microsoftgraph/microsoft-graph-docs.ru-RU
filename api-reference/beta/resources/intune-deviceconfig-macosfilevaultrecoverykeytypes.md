---
title: тип перечисления Макосфилеваултрековерикэйтипес
description: Типы ключей восстановления для macOS Филеваулт
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b53726b04dcecd1411caa1cee2f6e03638e30007
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42789473"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="6ec01-103">тип перечисления Макосфилеваултрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="6ec01-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

> <span data-ttu-id="6ec01-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ec01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ec01-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ec01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ec01-106">Типы ключей восстановления для macOS Филеваулт</span><span class="sxs-lookup"><span data-stu-id="6ec01-106">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="6ec01-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6ec01-107">Members</span></span>
|<span data-ttu-id="6ec01-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6ec01-108">Member</span></span>|<span data-ttu-id="6ec01-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6ec01-109">Value</span></span>|<span data-ttu-id="6ec01-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ec01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ec01-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6ec01-111">notConfigured</span></span>|<span data-ttu-id="6ec01-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6ec01-112">0</span></span>|<span data-ttu-id="6ec01-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="6ec01-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="6ec01-114">институтионалрековерикэй</span><span class="sxs-lookup"><span data-stu-id="6ec01-114">institutionalRecoveryKey</span></span>|<span data-ttu-id="6ec01-115">1,1</span><span class="sxs-lookup"><span data-stu-id="6ec01-115">1</span></span>|<span data-ttu-id="6ec01-116">Ключ восстановления для сотрудников в учреждений — это "главный" ключ восстановления, который можно использовать для разблокировки устройств, пароли которых были утрачены.</span><span class="sxs-lookup"><span data-stu-id="6ec01-116">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="6ec01-117">персоналрековерикэй</span><span class="sxs-lookup"><span data-stu-id="6ec01-117">personalRecoveryKey</span></span>|<span data-ttu-id="6ec01-118">2</span><span class="sxs-lookup"><span data-stu-id="6ec01-118">2</span></span>|<span data-ttu-id="6ec01-119">Персональный ключ восстановления — это уникальный код, который можно использовать для разблокировки устройства пользователя даже в том случае, если пароль для устройства утерян.</span><span class="sxs-lookup"><span data-stu-id="6ec01-119">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|



