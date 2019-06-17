---
title: тип перечисления Макосфилеваултрековерикэйтипес
description: Типы ключей восстановления для macOS Филеваулт
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 193bfc5769da2919f93df9beef38524a57bfece0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002548"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="dd541-103">тип перечисления Макосфилеваултрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="dd541-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

> <span data-ttu-id="dd541-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd541-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd541-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd541-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd541-106">Типы ключей восстановления для macOS Филеваулт</span><span class="sxs-lookup"><span data-stu-id="dd541-106">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="dd541-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="dd541-107">Members</span></span>
|<span data-ttu-id="dd541-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="dd541-108">Member</span></span>|<span data-ttu-id="dd541-109">Значение</span><span class="sxs-lookup"><span data-stu-id="dd541-109">Value</span></span>|<span data-ttu-id="dd541-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dd541-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd541-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="dd541-111">notConfigured</span></span>|<span data-ttu-id="dd541-112">нуль</span><span class="sxs-lookup"><span data-stu-id="dd541-112">0</span></span>|<span data-ttu-id="dd541-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="dd541-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="dd541-114">Институтионалрековерикэй</span><span class="sxs-lookup"><span data-stu-id="dd541-114">institutionalRecoveryKey</span></span>|<span data-ttu-id="dd541-115">1,1</span><span class="sxs-lookup"><span data-stu-id="dd541-115">1</span></span>|<span data-ttu-id="dd541-116">Ключ восстановления для сотрудников в учреждений — это "главный" ключ восстановления, который можно использовать для разблокировки устройств, пароли которых были утрачены.</span><span class="sxs-lookup"><span data-stu-id="dd541-116">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="dd541-117">Персоналрековерикэй</span><span class="sxs-lookup"><span data-stu-id="dd541-117">personalRecoveryKey</span></span>|<span data-ttu-id="dd541-118">2</span><span class="sxs-lookup"><span data-stu-id="dd541-118">2</span></span>|<span data-ttu-id="dd541-119">Персональный ключ восстановления — это уникальный код, который можно использовать для разблокировки устройства пользователя даже в том случае, если пароль для устройства утерян.</span><span class="sxs-lookup"><span data-stu-id="dd541-119">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|





