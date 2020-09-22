---
title: тип перечисления Макосфилеваултрековерикэйтипес
description: Типы ключей восстановления для macOS Филеваулт
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: df4374cdcb56a4400c483fea84d2cf02b3c6c0dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024173"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="94cd6-103">тип перечисления Макосфилеваултрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="94cd6-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

<span data-ttu-id="94cd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94cd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94cd6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94cd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94cd6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94cd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94cd6-107">Типы ключей восстановления для macOS Филеваулт</span><span class="sxs-lookup"><span data-stu-id="94cd6-107">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="94cd6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="94cd6-108">Members</span></span>
|<span data-ttu-id="94cd6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="94cd6-109">Member</span></span>|<span data-ttu-id="94cd6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="94cd6-110">Value</span></span>|<span data-ttu-id="94cd6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="94cd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94cd6-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="94cd6-112">notConfigured</span></span>|<span data-ttu-id="94cd6-113">нуль</span><span class="sxs-lookup"><span data-stu-id="94cd6-113">0</span></span>|<span data-ttu-id="94cd6-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="94cd6-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="94cd6-115">институтионалрековерикэй</span><span class="sxs-lookup"><span data-stu-id="94cd6-115">institutionalRecoveryKey</span></span>|<span data-ttu-id="94cd6-116">1 </span><span class="sxs-lookup"><span data-stu-id="94cd6-116">1</span></span>|<span data-ttu-id="94cd6-117">Ключ восстановления для сотрудников в учреждений — это "главный" ключ восстановления, который можно использовать для разблокировки устройств, пароли которых были утрачены.</span><span class="sxs-lookup"><span data-stu-id="94cd6-117">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="94cd6-118">персоналрековерикэй</span><span class="sxs-lookup"><span data-stu-id="94cd6-118">personalRecoveryKey</span></span>|<span data-ttu-id="94cd6-119">2 </span><span class="sxs-lookup"><span data-stu-id="94cd6-119">2</span></span>|<span data-ttu-id="94cd6-120">Персональный ключ восстановления — это уникальный код, который можно использовать для разблокировки устройства пользователя даже в том случае, если пароль для устройства утерян.</span><span class="sxs-lookup"><span data-stu-id="94cd6-120">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|






