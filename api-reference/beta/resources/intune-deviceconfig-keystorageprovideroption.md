---
title: Тип перечисления keyStorageProviderOption
description: Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424226"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="5beee-103">Тип перечисления keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="5beee-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="5beee-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5beee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5beee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5beee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5beee-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5beee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5beee-107">Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).</span><span class="sxs-lookup"><span data-stu-id="5beee-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="5beee-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5beee-108">Members</span></span>
|<span data-ttu-id="5beee-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5beee-109">Member</span></span>|<span data-ttu-id="5beee-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5beee-110">Value</span></span>|<span data-ttu-id="5beee-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5beee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5beee-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="5beee-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="5beee-113">0</span><span class="sxs-lookup"><span data-stu-id="5beee-113">0</span></span>|<span data-ttu-id="5beee-114">Импорта для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — импорт поставщика хранилища КЛЮЧЕЙ программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="5beee-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="5beee-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="5beee-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="5beee-116">1</span><span class="sxs-lookup"><span data-stu-id="5beee-116">1</span></span>|<span data-ttu-id="5beee-117">Импорт для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — не удается.</span><span class="sxs-lookup"><span data-stu-id="5beee-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="5beee-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="5beee-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="5beee-119">2</span><span class="sxs-lookup"><span data-stu-id="5beee-119">2</span></span>|<span data-ttu-id="5beee-120">Импорт Passport для работы поставщика хранилища КЛЮЧЕЙ Если доступно, в противном случае — ошибка.</span><span class="sxs-lookup"><span data-stu-id="5beee-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="5beee-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="5beee-121">useSoftwareKsp</span></span>|<span data-ttu-id="5beee-122">3</span><span class="sxs-lookup"><span data-stu-id="5beee-122">3</span></span>|<span data-ttu-id="5beee-123">Импорт на программное обеспечение поставщика хранилища КЛЮЧЕЙ.</span><span class="sxs-lookup"><span data-stu-id="5beee-123">Import to Software KSP.</span></span>|




