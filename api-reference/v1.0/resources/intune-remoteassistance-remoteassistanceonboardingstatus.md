---
title: тип переименовки remoteAssistanceOnboardingStatus
description: Текущее состояние соединиттеля TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ddd6d2884ef44a70f424de6d7e23d6bd6a3e94d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60448950"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>тип переименовки remoteAssistanceOnboardingStatus

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Текущее состояние соединиттеля TeamViewer

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notOnboarded|0|Состояние, сообщаемое при отсутствие активного соединитетеля TeamViewer, настроенного или активного|
|onboarding|1|Состояние, сообщалось, когда система инициировала подключение TeamViewer, но служба еще не завершила подтверждение соединитетеля|
|onboarded|2|Состояние, о чем сообщалось, когда система успешно обменивалась сведениями о учетных записях с TeamViewer и теперь может инициировать сеансы удаленной помощи с клиентами|



