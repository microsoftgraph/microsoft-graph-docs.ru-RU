---
title: тип перечисления Макосфилеваултрековерикэйтипес
description: Типы ключей восстановления для macOS Филеваулт
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1a72cc8ddb4e9ce28a65e3af006ebec097eda247
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365057"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="32862-103">тип перечисления Макосфилеваултрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="32862-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

> <span data-ttu-id="32862-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32862-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32862-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32862-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32862-106">Типы ключей восстановления для macOS Филеваулт</span><span class="sxs-lookup"><span data-stu-id="32862-106">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="32862-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="32862-107">Members</span></span>
|<span data-ttu-id="32862-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="32862-108">Member</span></span>|<span data-ttu-id="32862-109">Значение</span><span class="sxs-lookup"><span data-stu-id="32862-109">Value</span></span>|<span data-ttu-id="32862-110">Описание</span><span class="sxs-lookup"><span data-stu-id="32862-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32862-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="32862-111">notConfigured</span></span>|<span data-ttu-id="32862-112">нуль</span><span class="sxs-lookup"><span data-stu-id="32862-112">0</span></span>|<span data-ttu-id="32862-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="32862-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="32862-114">институтионалрековерикэй</span><span class="sxs-lookup"><span data-stu-id="32862-114">institutionalRecoveryKey</span></span>|<span data-ttu-id="32862-115">1,1</span><span class="sxs-lookup"><span data-stu-id="32862-115">1</span></span>|<span data-ttu-id="32862-116">Ключ восстановления для сотрудников в учреждений — это "главный" ключ восстановления, который можно использовать для разблокировки устройств, пароли которых были утрачены.</span><span class="sxs-lookup"><span data-stu-id="32862-116">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="32862-117">персоналрековерикэй</span><span class="sxs-lookup"><span data-stu-id="32862-117">personalRecoveryKey</span></span>|<span data-ttu-id="32862-118">2</span><span class="sxs-lookup"><span data-stu-id="32862-118">2</span></span>|<span data-ttu-id="32862-119">Персональный ключ восстановления — это уникальный код, который можно использовать для разблокировки устройства пользователя даже в том случае, если пароль для устройства утерян.</span><span class="sxs-lookup"><span data-stu-id="32862-119">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|



