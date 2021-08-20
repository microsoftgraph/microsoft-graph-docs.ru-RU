---
title: тип enum windowsDefenderProductStatus
description: Состояние продукта Защитник Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 17a5854c2579a039012b31950cce8660f6031a8c3048e437ffc52e94f6a18f23
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122413"
---
# <a name="windowsdefenderproductstatus-enum-type"></a>тип enum windowsDefenderProductStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние продукта Защитник Windows

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|noStatus|0|Отсутствие состояния|
|serviceNotRunning|1 |Не запущенная служба|
|serviceStartedWithoutMalwareProtection|2|Служба началась без какого-либо двигателя защиты от вредоносных программ|
|pendingFullScanDueToThreatAction|4 |Ожидание полного сканирования из-за действия угрозы|
|pendingRebootDueToThreatAction|8 |Ожидание перезагрузки из-за действия угрозы|
|pendingManualStepsDueToThreatAction|16 |Ожидание действий вручную из-за действия угрозы |
|avSignaturesOutOfDate|32|Подписи AV устарели|
|asSignaturesOutOfDate|64|As signatures out of date|
|noQuickScanHappenedForSpecifiedPeriod|128|Быстрого сканирования за указанный период не произошло|
|noFullScanHappenedForSpecifiedPeriod|256|Полное сканирование не было за указанный период|
|systemInitiatedScanInProgress|512|Начатое системное сканирование в процессе|
|systemInitiatedCleanInProgress|1024|Система инициировала очистку в процессе выполнения|
|samplesPendingSubmission|2048|Есть примеры, ожидающих отправки|
|productRunningInEvaluationMode|4096|Продукт, запущенный в режиме оценки|
|productRunningInNonGenuineMode|8192|Продукт, работающий в неподдельном Windows режиме|
|productExpired|16384|Срок действия продукта истек|
|offlineScanRequired|32768|Off-line scan required|
|serviceShutdownAsPartOfSystemShutdown|65536|Служба закрывается в рамках отключения системы|
|threatRemediationFailedCritically|131072|Исправление угрозы не удалось критически|
|threatRemediationFailedNonCritically|262144|Устранение угрозы не удалось без критических последствий|
|noStatusFlagsSet|524288|Нет набора флагов состояния (хорошо инициализированное состояние)|
|platformOutOfDate|1048576|Платформа устарела|
|platformUpdateInProgress|2097152|Обновление платформы продолжается|
|platformAboutToBeOutdated|4194304|Платформа вот-вот устареет|
|signatureOrPlatformEndOfLifeIsPastOrIsImpending|8388608|Подпись или окончание жизни платформы прошло или надвигается|
|windowsSModeSignaturesInUseOnNonWin10SInstall|16777216|Windows Сигнатуры SMode, которые по-прежнему используются при установке non-Win10S|




