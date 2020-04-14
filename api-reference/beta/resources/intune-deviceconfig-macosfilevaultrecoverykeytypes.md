---
title: тип перечисления Макосфилеваултрековерикэйтипес
description: Типы ключей восстановления для macOS Филеваулт
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 77fe5f115fec13498d0dbd034d87872f65bfc211
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383456"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="f18db-103">тип перечисления Макосфилеваултрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="f18db-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

<span data-ttu-id="f18db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f18db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f18db-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f18db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f18db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f18db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f18db-107">Типы ключей восстановления для macOS Филеваулт</span><span class="sxs-lookup"><span data-stu-id="f18db-107">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="f18db-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f18db-108">Members</span></span>
|<span data-ttu-id="f18db-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f18db-109">Member</span></span>|<span data-ttu-id="f18db-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f18db-110">Value</span></span>|<span data-ttu-id="f18db-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f18db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f18db-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f18db-112">notConfigured</span></span>|<span data-ttu-id="f18db-113">нуль</span><span class="sxs-lookup"><span data-stu-id="f18db-113">0</span></span>|<span data-ttu-id="f18db-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="f18db-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="f18db-115">институтионалрековерикэй</span><span class="sxs-lookup"><span data-stu-id="f18db-115">institutionalRecoveryKey</span></span>|<span data-ttu-id="f18db-116">1,1</span><span class="sxs-lookup"><span data-stu-id="f18db-116">1</span></span>|<span data-ttu-id="f18db-117">Ключ восстановления для сотрудников в учреждений — это "главный" ключ восстановления, который можно использовать для разблокировки устройств, пароли которых были утрачены.</span><span class="sxs-lookup"><span data-stu-id="f18db-117">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="f18db-118">персоналрековерикэй</span><span class="sxs-lookup"><span data-stu-id="f18db-118">personalRecoveryKey</span></span>|<span data-ttu-id="f18db-119">2</span><span class="sxs-lookup"><span data-stu-id="f18db-119">2</span></span>|<span data-ttu-id="f18db-120">Персональный ключ восстановления — это уникальный код, который можно использовать для разблокировки устройства пользователя даже в том случае, если пароль для устройства утерян.</span><span class="sxs-lookup"><span data-stu-id="f18db-120">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|



