---
title: Отчеты об активации Microsoft 365
description: Отчеты об активации Microsoft 365 могут предоставить представление о том, какие пользователи активировали подписки Microsoft 365 по крайней мере на одном устройстве. В этих отчетах представлены сведения об активации подписки на Microsoft 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах. Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 34bebb8edb7d83ca631d93add90a7e2810849c3d
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898172"
---
# <a name="microsoft-365-activations-reports"></a>Отчеты об активации Microsoft 365

Пространство имен: microsoft.graph

Отчеты об активации Microsoft 365 могут предоставить представление о том, какие пользователи активировали подписки Microsoft 365 по крайней мере на одном устройстве. В этих отчетах представлены сведения об активации подписки на Microsoft 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах. Эти отчеты помогут вам выявить пользователей, которым, возможно, нужна помощь с активацией подписки на Office.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports — активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Отчеты
| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activationsuserdetail.md) | Stream      | Получение сведений о пользователях, которые активировали Microsoft 365. |
| [Получение количества активаций](../api/reportroot-getoffice365activationcounts.md) | Поток      | Получение числа активаций Microsoft 365 на настольных компьютерах и устройствах. |
| [Получение количества пользователей](../api/reportroot-getoffice365activationsusercounts.md) | Stream      | Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве. |
